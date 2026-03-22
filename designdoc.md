Company Name: Demarka
Business Model: Demarka is a B2B SaaS platform for trademark search and monitoring. We offer monthly subscriptions and one-time search services to lawyers, startups, and business owners. Our website is demarka.eu.

Tool Access/Use: Our tool will be used internally by our marketing team to manage and optimize Google Ads campaigns. The tool is an AI assistant (Claude via MCP) that allows our team to create campaigns, manage ad groups, adjust bids, and pull performance reports through natural language commands. Third parties do not receive Google Ads credentials or direct API access; natural-language processing may be performed by our AI provider under our configuration. All Google Ads operations target our own customer account(s) only.

Tool Design: The tool connects Claude AI to the Google Ads API via Model Context Protocol (MCP). Our marketing team interacts with Claude in natural language to perform campaign operations. Claude translates these requests into Google Ads API v20 calls through the official Python client. The MCP server exposes tools that map to the API services listed below.

API Services Called (Google Ads API v20):

The MCP implementation may invoke any of the following gRPC services, depending on the task (including GAQL search/stream via GoogleAdsService and field metadata via GoogleAdsFieldService):

- AccountBudgetProposalService
- AccountLinkService
- AdGroupAdLabelService
- AdGroupAdService
- AdGroupAssetService
- AdGroupAssetSetService
- AdGroupBidModifierService
- AdGroupCriterionCustomizerService
- AdGroupCriterionLabelService
- AdGroupCriterionService
- AdGroupCustomizerService
- AdGroupLabelService
- AdGroupService
- AdParameterService
- AssetGroupAssetService
- AssetGroupService
- AssetGroupSignalService
- AssetService
- AssetSetService
- AudienceInsightsService
- AudienceService
- BatchJobService
- BiddingDataExclusionService
- BiddingSeasonalityAdjustmentService
- BiddingStrategyService
- BillingSetupService
- BrandSuggestionService
- CampaignAssetService
- CampaignAssetSetService
- CampaignBidModifierService
- CampaignBudgetService
- CampaignConversionGoalService
- CampaignCriterionService
- CampaignCustomizerService
- CampaignDraftService
- CampaignLabelService
- CampaignService
- CampaignSharedSetService
- ConversionActionService
- ConversionAdjustmentUploadService
- ConversionCustomVariableService
- ConversionGoalCampaignConfigService
- ConversionUploadService
- ConversionValueRuleService
- CustomAudienceService
- CustomConversionGoalService
- CustomInterestService
- CustomerAssetService
- CustomerClientLinkService
- CustomerConversionGoalService
- CustomerCustomizerService
- CustomerLabelService
- CustomerManagerLinkService
- CustomerNegativeCriterionService
- CustomerService
- CustomerUserAccessInvitationService
- CustomerUserAccessService
- CustomizerAttributeService
- DataLinkService
- ExperimentArmService
- ExperimentService
- GeoTargetConstantService
- GoogleAdsFieldService
- GoogleAdsService
- IdentityVerificationService
- InvoiceService
- KeywordPlanAdGroupKeywordService
- KeywordPlanAdGroupService
- KeywordPlanCampaignKeywordService
- KeywordPlanCampaignService
- KeywordPlanIdeaService
- KeywordPlanService
- LabelService
- OfflineUserDataJobService
- PaymentsAccountService
- ProductLinkService
- ReachPlanService
- RecommendationService
- RemarketingActionService
- SharedCriterionService
- SharedSetService
- SmartCampaignSuggestService
- UserDataService
- UserListService

Tool Mockups: We use Claude Cowork as the primary interface (conversational UI). No separate custom web dashboard; a screenshot of a sample session in that environment can be provided if required for external review.
