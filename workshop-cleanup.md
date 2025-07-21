# 🧹 Workshop Cleanup Guide
*Clean up your AWS resources to avoid unnecessary charges*

## Why Cleanup Matters 💰

While AWS Bedrock charges are usage-based (you only pay for what you generate), S3 storage incurs ongoing monthly charges. Let's clean up workshop resources to keep your AWS account tidy and avoid surprise bills!

## Cleanup Checklist ✅

### 1. Delete S3 Bucket and Contents (5 min)

Your Nova Reel videos are stored in S3, which charges for storage. Here's how to remove them:

#### Step 1: Navigate to S3
1. **Open** AWS Console: https://console.aws.amazon.com
2. **Search for** "S3" in the top search bar
3. **Click** "S3" to open the service

#### Step 2: Empty Your Workshop Bucket
1. **Find your bucket**: `nova-reel-workshop-[your-name]`
2. **Click** on the bucket name
3. **Select all objects** (checkbox at top)
4. **Click** "Delete" button
5. **Type** "permanently delete" in the confirmation box
6. **Click** "Delete objects"

#### Step 3: Delete the Bucket
1. **Return** to S3 bucket list (click "Amazon S3" in breadcrumb)
2. **Select** your workshop bucket (checkbox)
3. **Click** "Delete" button
4. **Type** your bucket name to confirm
5. **Click** "Delete bucket"

### 2. Check for Leftover Generated Content (2 min)

#### Bedrock Playground History
Bedrock Playgrounds don't store content long-term, but you should:
1. **Save any prompts** you want to keep in your personal notes
2. **Download any images** you want to preserve
3. **Note:** Text responses aren't stored after session ends

### 3. Cost Verification (2 min)

#### Check Your Usage
1. **Navigate to** AWS Billing Dashboard
2. **Click** "Bills" in left sidebar
3. **Expand** "Amazon Bedrock" to see generation costs
4. **Expand** "Amazon S3" to see storage costs
5. **Verify** costs align with workshop usage

#### Set Up Billing Alerts (Optional but Recommended)
1. **In Billing Dashboard**, click "Budgets"
2. **Create budget** with $10 monthly limit
3. **Set alert** at 80% threshold
4. **Add your email** for notifications

### 4. Workshop Assets Organization (5 min)

#### Save Your Work Locally
Before cleanup, ensure you've saved:
- [ ] Successful prompts in a text document
- [ ] Generated images you want to keep
- [ ] Downloaded videos from S3
- [ ] Campaign materials created
- [ ] Screenshots of favorite outputs

#### Recommended Folder Structure:
```
Nova-Workshop-Outputs/
├── Prompts/
│   ├── text-prompts.txt
│   ├── image-prompts.txt
│   └── video-prompts.txt
├── Images/
│   ├── hero-images/
│   ├── social-media/
│   └── backgrounds/
├── Videos/
│   ├── campaign-hero.mp4
│   ├── social-teasers/
│   └── feature-demos/
└── Final-Campaign/
    ├── taglines.txt
    ├── visuals/
    └── videos/
```

## Important Reminders ⚠️

### S3 Storage Costs
- **Videos remain in S3** until you delete them
- **Storage costs** ~$0.023 per GB per month
- **A 10-second video** is typically 5-20MB
- **100 videos** ≈ 1-2GB ≈ $0.02-0.05/month
- **Still adds up** if forgotten!

### Bedrock Costs
- **Usage-based** - no ongoing charges
- **No cleanup needed** for Bedrock itself
- **Charges stop** when you stop generating

### AWS Free Tier
- **Some S3 storage** included in free tier
- **First 5GB** free for 12 months (new accounts)
- **After free tier**, standard rates apply

## Quick Cleanup Script (Advanced) 🚀

For those comfortable with AWS CLI:

```bash
# List all objects in bucket
aws s3 ls s3://nova-reel-workshop-[your-name]/ --recursive

# Download all videos locally (optional)
aws s3 sync s3://nova-reel-workshop-[your-name]/ ./workshop-backup/

# Remove all objects and bucket
aws s3 rb s3://nova-reel-workshop-[your-name]/ --force
```

## Final Checks ✅

Before leaving:
- [ ] S3 bucket deleted
- [ ] Important outputs saved locally
- [ ] Prompts documented
- [ ] Billing alerts set (optional)
- [ ] Team shared assets (if applicable)

## Keep Learning! 🎓

### What NOT to Delete:
- **Your AWS account** - Keep it for future projects!
- **Bedrock access** - No cost when not in use
- **Your learnings** - The most valuable output!

### Next Steps:
1. **Practice** with your own projects
2. **Share** your creations
3. **Join** the community
4. **Keep experimenting** with AI

## Questions? 

### Common Cleanup Issues:

**"Bucket not empty" error:**
- Make sure all objects are deleted first
- Check for hidden files (versions, markers)
- Use "Empty bucket" option before deleting

**"Access denied" error:**
- Verify you're in the correct AWS account
- Check you're in the right region
- Ensure you have deletion permissions

**Can't find my bucket:**
- Check all regions (top-right dropdown)
- Search by partial name
- Check CloudTrail for creation region

---

## Thank You! 🙏

Thanks for participating in the Nova Creative Studio Workshop! 

Remember:
- **Cleanup is self-service** - AWS won't do it automatically
- **S3 charges are monthly** - delete buckets you don't need
- **Bedrock has no ongoing costs** - only pay when generating

Happy creating with AI! 🎨🚀

---

*Workshop cleanup typically takes 5-10 minutes. Do it now while it's fresh in your mind!*