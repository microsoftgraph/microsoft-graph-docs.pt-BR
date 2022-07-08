---
title: Valores de enumeração
description: Valores de enumeração do Microsoft Graph
doc_type: enumPageType
ms.localizationpriority: medium
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: dd17d54c0d6cd991f02a5043765aab199bfc3a05
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690067"
---
# <a name="enum-values"></a>Valores de enumeração

Namespace: microsoft.graph


### <a name="teamtemplateaudience-values"></a>Valores de teamTemplateAudience 

|Member|
|:---|
|organization|
|user|
|public|
|unknownFutureValue|

### <a name="decisionitemprincipalresourcemembershiptype-values"></a>Valores decisionItemPrincipalResourceMembershipType 

|Member|
|:---|
|Direto|
|Indireta|
|unknownFutureValue|

### <a name="signinfrequencyauthenticationtype-values"></a>Valores signInFrequencyAuthenticationType

|Member|
|:---|
|primaryAndSecondaryAuthentication|
|secondaryAuthentication|
|unknownFutureValue|

### <a name="signinfrequencyinterval-values"></a>Valores signInFrequencyInterval

|Member|
|:---|
|timeBased|
|Sempre|

#### <a name="authenticationprotocol-values"></a>Valores authenticationProtocol

|Member|
|:---|
|wsFed|
|Saml|
|unknownFutureValue|

#### <a name="federatedidpmfabehavior-values"></a>Valores federatedIdpMfaBehavior
|Member|
|:---|
|acceptIfMfaDoneByFederatedIdp|
|enforceMfaByFederatedIdp|
|rejectMfaByFederatedIdp|
|unknownFutureValue|

#### <a name="promptloginbehavior-values"></a>Valores de promptLoginBehavior
|Member|
|:---|
|translateToFreshPasswordAuthentication|
|nativeSupport|
|desabilitadas|
|unknownFutureValue|

### <a name="bookingsavailabilitystatus-values"></a>valores bookingsAvailabilityStatus

|Member|
|:-----|
|disponível|
|Ocupado|
|slotsAvailable|
|outOfOffice|
|unknownFutureValue|

### <a name="accesspackagecustomextensionhandlerstatus-values"></a>Valores de accessPackageCustomExtensionHandlerStatus 

|Member|
|:---|
|requestSent|
|requestReceived|
|unknownFutureValue|

### <a name="accesspackagecustomextensionstage-values"></a>valores accessPackageCustomExtensionStage 

|Member|
|:---|
|assignmentRequestCreated|
|assignmentRequestApproved|
|assignmentRequestGranted|
|assignmentRequestRemoved|
|assignmentFourteenDaysBeforeExpiration|
|assignmentOneDayBeforeExpiration|
|unknownFutureValue|

### <a name="accessreviewhistorystatus-values"></a>valores accessReviewHistoryStatus

| Member|
|:-----------------|
|done|
|Inprogress|
|erro|
|Solicitado|
|unknownFutureValue|

### <a name="accessreviewhistorydecisionfilter-values"></a>valores accessReviewHistoryDecisionFilter

| Member|
|:-----------------|
|Aprovar|
|Negar|
|notReviewed|
|dontKnow|
|notNotified|
|unknownFutureValue|


### <a name="accessreviewhistorystatus-values"></a>valores accessReviewHistoryStatus

|Member|
|:---|
|done|
|Inprogress|
|erro|
|Solicitado|
|unknownFutureValue|

### <a name="crosstenantaccesspolicytargetconfigurationaccesstype-values"></a>Valores crossTenantAccessPolicyTargetConfigurationAccessType

|Member|
|:---|
|Permitido|
|Bloqueado|
|unknownFutureValue|

### <a name="crosstenantaccesspolicytargettype-values"></a>Valores crossTenantAccessPolicyTargetType

|Member|
|:---|
|user|
|group|

### <a name="accesspackagefilterbycurrentuseroptions-values"></a>Valores de accessPackageFilterByCurrentUserOptions

|Member|
|:---|
|allowedRequestor|
|unknownFutureValue|

### <a name="usersigninrecommendationscope-values"></a>Valores userSignInRecommendationScope 

|Member|
|:---|
|locatário|
|aplicação|

### <a name="incomingtokentype-values"></a>Valores incomingTokenType 

|Member|
|:---|
|none|
|primaryRefreshToken|
|saml11|
|saml20|
|unknownFutureValue|
|remoteDesktopToken|

### <a name="protocoltype-values"></a>valores protocolType 

|Member|
|:---|
|none|
|oAuth2|
|ropc|
|wsFederation|
|saml20|
|deviceCode|
|unknownFutureValue|

### <a name="accessreviewinstancedecisionitemfilterbycurrentuseroptions-values"></a>Valores de accessReviewInstanceDecisionItemFilterByCurrentUserOptions 

|Member|
|:---|
|Revisor|
|unknownFutureValue|

### <a name="accessreviewstagefilterbycurrentuseroptions-values"></a>Valores accessReviewStageFilterByCurrentUserOptions 

|Member|
|:---|
|Revisor|
|unknownFutureValue|

### <a name="continuousaccessevaluationmode-values"></a>Valores continuousAccessEvaluationMode 

|Member|
|:---|
|strictEnforcement|
|desabilitadas|
|unknownFutureValue|

### <a name="multifactorauthconfiguration-values"></a>Valores multiFactorAuthConfiguration

| Membro             | Valor | Descrição |
|:-------------------|:------| :------|
| notRequired        | 0     | Nenhuma autenticação multifator é necessária para que um usuário conclua o registro do dispositivo.|
| obrigatório           | 1     | A autenticação multifator é necessária para que um usuário conclua o registro do dispositivo.|
| unknownFutureValue | 2     | Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="policyscope-values"></a>Valores de policyScope

| Membro             | Valor | Descrição |
|:-------------------|:------| :------|
| none               | 0     | A política não se aplica a nenhum usuário ou grupo na organização. |
| tudo                | 1     | A política se aplica a todos os usuários e grupos na organização. Valor padrão. |
| Selecionado           | 2     | A política se aplica a usuários ou grupos específicos na organização. |
| unknownFutureValue | 3     | Valor de sentinel de enumeração evolvável. Não usar. |

### <a name="appcredentialrestrictiontype-values"></a>Valores appCredentialRestrictionType

| Member                 |
| :--------------------- |
| passwordAddition       |
| passwordLifetime       |
| symmetricKeyAddition   |
| symmetricKeyLifetime   |
| customPasswordAddition |
| unknownFutureValue     |

### <a name="appkeycredentialrestrictiontype-values"></a>Valores appKeyCredentialRestrictionType

|Member|
|:-----|
|asymmetricKeyLifetime|
|unknownFutureValue|

### <a name="synchronizationsecret-values"></a>valores synchronizationSecret

|Member|
|:----|
|Nenhum|
|UserName|
|Password|
|SecretToken|
|AppKey|
|Baseaddress|
|ClientIdentifier|
|ClientSecret|
|SingleSignOnType|
|Área restrita|
|Url|
|Domínio|
|ConsumerKey|
|ConsumerSecret|
|TokenKey|
|TokenExpiration|
|Oauth2AccessToken|
|Oauth2AccessTokenCreationTime|
|Oauth2RefreshToken|
|SyncAll|
|Instancename|
|Oauth2ClientId|
|Oauth2ClientSecret|
|CompanyId|
|UpdateKeyOnSoftDelete|
|SynchronizationSchedule|
|SystemOfRecord|
|SandboxName|
|EnforceDomain|
|SyncNotificationSettings|
|SkipOutOfScopeDeletions|
|Oauth2AuthorizationCode|
|Oauth2RedirectUri|
|ApplicationTemplateIdentifier|
|Servidor|
|PerformInboundEntitlementGrants|
|HardDeletesEnabled|
|SyncAgentCompatibilityKey|
|SyncAgentADContainer|
|ValidateDomain|
|TestReferences|

### <a name="filtermode-values"></a>Valores filterMode

|Member|
|:---|
|Incluem|
|Excluir|

### <a name="lifecycleeventtype-values"></a>Valores lifecycleEventType

|Member|
|:---|
|Perdeu|
|subscriptionRemoved|
|reauthorizationRequired|

### <a name="changetype-values"></a>Valores changeType

|Member|
|:---|
|criadas|
|Atualizado|
|deleted|


### <a name="countrylookupmethodtype-values"></a>valores countryLookupMethodType

|Member|
|:---|
|clientIpAddress|
|authenticatorAppGps|

### <a name="approvalstate-values"></a>Valores approvalState

|Member|
|:---|
|Pendente|
|Aprovado|
|denied|
|Abortado|
|Cancelado|

### <a name="rolesummarystatus-values"></a>Valores roleSummaryStatus

|Member|
|:---|
|Okey|
|Ruim|

### <a name="datapolicyoperationstatus-values"></a>Valores de dataPolicyOperationStatus

|Member|
|:---|
|Notstarted|
|Executando|
|complete|
|Falhou|
|unknownFutureValue|

### <a name="conditionalaccessclientapp-values"></a>Valores de conditionalAccessClientApp

|Member|
|:---|
|tudo|
|Navegador|
|mobileAppsAndDesktopClients|
|exchangeActiveSync|
|easSupported|
|Outros|

### <a name="consentrequestfilterbycurrentuseroptions-values"></a>Valores consentRequestFilterByCurrentUserOptions

|Member|
|:---|
|Revisor|
|unknownFutureValue|

### <a name="attributetype-values"></a>Valores attributeType

|Member|
|:---|
|Cadeia de Caracteres|
|Inteiro|
|Referência|
|Binária|
|Booleano|
|DateTime|

### <a name="mutability-values"></a>valores de mutabilidade

|Member|
|:---|
|ReadWrite|
|ReadOnly|
|Imutável|
|Writeonly|

### <a name="directorydefinitiondiscoverabilities-values"></a>valores directoryDefinitionDiscoverabilities

|Member|
|:---|
|Nenhum|
|Attributenames|
|AttributeDataTypes|
|AttributeReadOnly|
|ReferenceAttributes|
|UnknownFutureValue|

### <a name="connectorgroupregion-values"></a>Valores connectorGroupRegion

|Member|
|:---|
|Nam|
|Euros|
|Aus|
|Ásia|
|Ind|
|unknownFutureValue|

### <a name="connectorgrouptype-values"></a>Valores connectorGroupType

|Member|
|:---|
|applicationProxy|

### <a name="onpremisespublishingtype-values"></a>valores onPremisesPublishingType

|Member|
|:---|
|applicationProxy|
|exchangeOnline|
|autenticação|
|Provisionamento|
|intunePfx|
|oflineDomainJoin|
|unknownFutureValue|

### <a name="agentstatus-values"></a>Valores agentStatus

|Member|
|:---|
|Ativo|
|Inativo|

### <a name="connectorstatus-values"></a>Valores connectorStatus

|Member|
|:---|
|Ativo|
|Inativo|

### <a name="calltype-values"></a>Valores callType

|Member|
|:---|
|desconhecido|
|groupCall|
|Peertopeer|
|unknownFutureValue|

### <a name="tone-values"></a>valores de tom

|Member|
|:---|
|tone0|
|tone1|
|tone2|
|tone3|
|tone4|
|tone5|
|tone6|
|tone7|
|tom8|
|tone9|
|Estrela|
|Libra|
|a|
|b|
|c|
|d|
|Flash|

### <a name="callstate-values"></a>Valores de callState

|Member|
|:---|
|Entrada|
|Estabelecer|
|Tocando|
|Estabelecido|
|Segurar|
|Transferência|
|transferAccepted|
|Redirecionando|
|Terminação|
|Terminada|

### <a name="routingpolicy-values"></a>Valores routingPolicy

|Member|
|:---|
|none|
|noMissedCall|
|disableForwardingExceptPhone|
|disableForwarding|
|preferSkypeForBusiness|
|unknownFutureValue|

### <a name="meetingcapabilities-values"></a>valores meetingCapabilities

|Member|
|:---|
|questionAndAnswer|
|unknownFutureValue|

### <a name="onlinemeetingrole-values"></a>Valores onlineMeetingRole

|Member|
|:---|
|attendee|
|Apresentador|
|Produtor|
|unknownFutureValue|

### <a name="autoadmitteduserstype-values"></a>Valores autoAdmittedUsersType

|Member|
|:---|
|everyoneInCompany|
|Todos|

### <a name="mediastate-values"></a>valores mediaState

|Member|
|:---|
|Ativo|
|Inativo|
|unknownFutureValue|

### <a name="calldirection-values"></a>valores de callDirection

|Member|
|:---|
|Entrada|
|Saída|

### <a name="modality-values"></a>valores de modalidade

|Member|
|:---|
|audio|
|video|
|videoBasedScreenSharing|
|data|
|screenSharing|
|unknownFutureValue|

### <a name="kerberossignonmappingattributetype-values"></a>Valores kerberosSignOnMappingAttributeType

|Member|
|:---|
|userPrincipalName|
|onPremisesUserPrincipalName|
|userPrincipalUsername|
|onPremisesUserPrincipalUsername|
|onPremisesSAMAccountName|

### <a name="externalauthenticationtype-values"></a>Valores externalAuthenticationType

|Member|
|:---|
|Passthru|
|aadPreAuthentication|

### <a name="recipientscopetype-values"></a>Valores recipientScopeType
|Member|
|:---|
|none|
|Interno|
|Externo|
|externalPartner|
|externalNonPartner|

### <a name="appliedconditionalaccesspolicyresult-values"></a>Valores appliedConditionalAccessPolicyResult

|Member|
|:---|
|sucesso|
|Falha|
|notApplied|
|notEnabled|
|desconhecido|
|unknownFutureValue|
|reportOnlySuccess|
|reportOnlyFailure|
|reportOnlyNotApplied|
|reportOnlyInterrupted|


### <a name="microsoftauthenticatorauthenticationmode-values"></a>Valores microsoftAuthenticatorAuthenticationMode



|Member|
|:---|
|qualquer|
|Empurrar|
|deviceBasedPush|


### <a name="authenticationmethodfeature-values"></a>Valores authenticationMethodFeature

|Member|
|:---|
|ssprRegistered|
|ssprEnabled|
|ssprCapable|
|passwordlessCapable|
|mfaCapable|


### <a name="authmethodstype-values"></a>valores authMethodsType

|Member|
|:---|
|email|
|mobileSMS|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appNotificationCode|
|appNotificationAndCode|
|appPassword|
|Fido|
|alternateMobilePhone|
|mobilePhoneAndSMS|
|unknownFutureValue|


### <a name="defaultmfamethodtype-values"></a>Valores defaultMfaMethodType 



|Member|
|:---|
|none|
|mobilePhone|
|alternateMobilePhone|
|officePhone|
|microsoftAuthenticatorPush|
|softwareOneTimePasscode|
|unknownFutureValue|


### <a name="clientcredentialtype-values"></a>Valores clientCredentialType 



|Member|
|:---|
|none|
|clientSecret|
|clientAssertion|
|federatedIdentityCredential|
|managedIdentity|
|certificado|
|unknownFutureValue|


### <a name="azureadlicensetype-values"></a>valores azureADLicenseType

|Member|
|:---|
|none|
|Livre|
|Basic|
|premiumP1|
|premiumP2|
|unknownFutureValue|

### <a name="conditionalaccessconditions-values"></a>Valores conditionalAccessConditions

|Member|
|:---|
|none|
|aplicação|
|usuários|
|devicePlatform|
|localização|
|clientType|
|signInRisk|
|userRisk|
|hora|
|deviceState|
|Cliente|
|ipAddressSeenByAzureAD|
|ipAddressSeenByResourceProvider|
|unknownFutureValue|
|servicePrincipals|
|servicePrincipalRisk|

### <a name="conditionalaccessstatus-values"></a>Valores conditionalAccessStatus

|Member|
|:---|
|sucesso|
|Falha|
|notApplied|
|unknownFutureValue|

### <a name="featuretype-values"></a>Valores featureType

|Member|
|:---|
|Registo|
|redefinir|
|unknownFutureValue|

### <a name="grouptype-values"></a>Valores groupType

|Member|
|:---|
|unifiedGroups|
|azureAD|
|unknownFutureValue|

### <a name="includeduserroles-values"></a>Valores includedUserRoles

|Member|
|:---|
|tudo|
|privilegedAdmin|
|Admin|
|user|
|unknownFutureValue|

### <a name="includedusertypes-values"></a>Valores includedUserTypes

|Member|
|:---|
|tudo|
|Membro|
|Convidado|
|unknownFutureValue|

### <a name="initiatortype-values"></a>valores de initiatorType

|Member|
|:---|
|user|
|aplicativo|
|sistema|
|unknownFutureValue|

### <a name="migrationstatus-values"></a>Valores migrationStatus

|Member|
|:---|
|Pronto|
|needsReview|
|additionalStepsRequired|
|unknownFutureValue|

### <a name="networktype-values"></a>valores networkType

|Member|
|:---|
|Intranet|
|Extranet|
|namedNetwork|
|Confiável|
|unknownFutureValue|

### <a name="operationresult-values"></a>Valores operationResult

|Member|
|:---|
|sucesso|
|Falha|
|timeout|
|unknownFutureValue|

### <a name="provisioningresult-values"></a>Valores de provisioningResult

|Member|
|:---|
|sucesso|
|Falha|
|Ignorada|
|warning|
|unknownFutureValue|

### <a name="provisioningsteptype-values"></a>valores de provisioningStepType

|Member|
|:---|
|Importação|
|Escopo|
|Correspondência|
|Processamento|
|referenceResolution|
|Exportação|
|unknownFutureValue|

### <a name="registrationauthmethod-values"></a>valores registrationAuthMethod

|Member|
|:---|
|email|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobilePhone|
|Fido|
|appPassword|
|unknownFutureValue|

### <a name="registrationstatustype-values"></a>valores registrationStatusType

|Member|
|:---|
|Registrado|
|habilitadas|
|Capaz|
|mfaRegistered|
|unknownFutureValue|


### <a name="signinidentifiertype-values"></a>Valores signInIdentifierType 

|Member|
|:---|
|userPrincipalName|
|phoneNumber|
|Proxyaddress|
|qrCode|
|onPremisesUserPrincipalName|
|unknownFutureValue|


### <a name="signinusertype-values"></a>Valores signInUserType 

|Member|
|:---|
|Membro|
|Convidado|
|unknownFutureValue|

### <a name="requirementprovider-values"></a>valores de requirementProvider 


|Member|
|:---|
|user|
|Solicitação|
|servicePrincipal|
|v1ConditionalAccess|
|multiConditionalAccess|
|tenantSessionRiskPolicy|
|accountCompromisePolicies|
|v1ConditionalAccessDependency|
|v1ConditionalAccessPolicyIdRequested|
|mfaRegistrationRequiredByIdentityProtectionPolicy|
|baselineProtection|
|mfaRegistrationRequiredByBaselineProtection|
|mfaRegistrationRequiredByMultiConditionalAccess|
|enforcedForCspAdmins|
|securityDefaults|
|mfaRegistrationRequiredBySecurityDefaults|
|proofUpCodeRequest|
|crossTenantOutboundRule|
|gpsLocationCondition|
|riskBasedPolicy|
|unknownFutureValue|


### <a name="riskdetail-values"></a>Valores riskDetail

|Member|
|:---|
|none|
|Interno|
|Externo|
|externalPartner|
|externalNonPartner|
|adminGeneratedTemporaryPassword|
|userPerformedSecuredPasswordChange|
|userPerformedSecuredPasswordReset|
|adminConfirmedSigninSafe|
|aiConfirmedSigninSafe|
|userPassedMFADrivenByRiskBasedPolicy|
|adminDismissedAllRiskForUser|
|adminConfirmedSigninCompromised|
|hidden|
|adminConfirmedUserCompromised|
|unknownFutureValue|
|adminConfirmedServicePrincipalCompromised|
|adminDismissedAllRiskForServicePrincipal|


<!-- maintenance comment: Do not delete enum delcaration for riskEventType until all properties of this type are marked as deleted. Dec 28, 2021: Pending eventTypes (in riskUserActivity) and riskType (in riskDetection)-->
### <a name="riskeventtype-values"></a>Valores riskEventType

|Member|
|:---|
|unlikelyTravel|
|anonymizedIPAddress|
|maliciousIPAddress|
|unfamiliarFeatures|
|malwareInfectedIPAddress|
|suspiciousIPAddress|
|leakedCredentials|
|investigationsThreatIntelligence|
|Genérico|
|adminConfirmedUserCompromised|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="usageauthmethod-values"></a>Valores usageAuthMethod

|Member|
|:---|
|email|
|mobileSMS|
|mobileCall|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobileCall|
|Fido|
|appPassword|
|unknownFutureValue|

### <a name="authenticationmethodkeystrength-values"></a>Valores authenticationMethodKeyStrength

|Member|
|:---|
|Normal|
|Fraco|
|desconhecido|

### <a name="authenticationcontextdetail-values"></a>Valores authenticationContextDetail

|Member|
|:---|
|obrigatório|
|previouslySatisfied|
|notApplicable|
|unknownFutureValue|

### <a name="educationaddedstudentaction-values"></a>Valores educationAddedStudentAction

|Member|
|:---|
|none|
|assignIfOpen|
|unknownFutureValue|

### <a name="educationaddtocalendaroptions-values"></a>valores educationAddToCalendarOptions
|Member|
|:---|
|none|
|studentsAndPublisher|
|studentsAndTeamOwners|
|unknownFutureValue|
|studentsOnly|

### <a name="educationassignmentstatus-values"></a>valores educationAssignmentStatus
|Member|
|:---|
|Projecto|
|Publicado|
|Atribuído|
|unknownFutureValue|

### <a name="educationsubmissionstatus-values"></a>valores educationSubmissionStatus
|Member|
|:---|
|Trabalhando|
|Enviada|
|Lançado|
|Retornado|
|unknownFutureValue|
|Reatribuída|

### <a name="educationfeedbackresourceoutcomestatus-values"></a>valores educationFeedbackResourceOutcomeStatus
|Member|
|:---|
|notPublished|
|pendingPublish|
|Publicado|
|failedPublish|
|unknownFutureValue|

### <a name="externalemailotpstate-values"></a>Valores externalEmailOtpState

|Member|
|:---|
|Padrão.|
|habilitadas|
|desabilitadas|
|unknownFutureValue|

### <a name="expirationrequirement-values"></a>valores expirationRequirement

|Member|
|:---|
|rememberMultifactorAuthenticationOnTrustedDevices|
|tenantTokenLifetimePolicy|
|audienceTokenLifetimePolicy|
|signInFrequencyPeriodicReauthentication|
|ngcMfa|
|signInFrequencyEveryTime|
|unknownFutureValue|


### <a name="replyrestriction-values"></a>Valores replyRestriction

| Member
|:--------------
| Todos
| authorAndModerators
| unknownFutureValue

### <a name="usernewmessagerestriction-values"></a>Valores userNewMessageRestriction

| Member
|:--------------
|Todos
|everyoneExceptGuests
|Moderadores
|unknownFutureValue

### <a name="volumetype-values"></a>valores volumeType

|Member|
|:---|
|operatingSystemVolume|
|fixedDataVolume|
|removableDataVolume|
|unknownFutureValue|

### <a name="allowedaudiences-values"></a>Valores allowedAudiences

|Member|
|:---|
|me|
|Família|
|contacts|
|groupMembers|
|organization|
|federatedOrganizations|
|Todos|
|unknownFutureValue|

### <a name="attestationlevel-values"></a>valores attestationLevel

|Member|
|:---|
|Atestado|
|notAttested|
|unknownFutureValue|

### <a name="emailtype-values"></a>valores emailType

|Member|
|:---|
|desconhecido|
|trabalho|
|pessoal|
|Principal|
|Outros|

### <a name="authenticationmethodsigninstate-values"></a>Valores authenticationMethodSignInState

|Member|
|:---|
|notSupported|
|notAllowedByPolicy|
|notEnabled|
|phoneNumberNotUnique|
|Pronto|
|notConfigured|
|unknownFutureValue|

### <a name="authenticationphonetype-values"></a>Valores authenticationPhoneType

|Member|
|:---|
|móvel|
|alternateMobile|
|Escritório|
|unknownFutureValue|


### <a name="authenticationmethodtargettype-values"></a>Valores authenticationMethodTargetType

|Member|
|:---|
|user|
|group|

### <a name="authenticationmethodstate-values"></a>Valores authenticationMethodState

|Member|
|:---|
|habilitadas|
|desabilitadas|

### <a name="fido2restrictionenforcementtype-values"></a>Valores fido2RestrictionEnforcementType

|Member|
|:---|
|Permitir|
|Bloco|
|unknownFutureValue|

### <a name="x509certificateauthenticationmode-values"></a>Valores x509CertificateAuthenticationMode
|Member|
|:---|
|x509CertificateSingleFactor|
|x509CertificateMultiFactor|
|unknownFutureValue|

### <a name="x509certificateruletype-values"></a>Valores x509CertificateRuleType
|Member|
|:---|
|issuerSubject|
|policyOID|
|unknownFutureValue|

### <a name="anniversarytype-values"></a>valores anniversaryType

|Member|
|:---|
|birthday|
|Casamento|
|unknownFutureValue|

### <a name="skillproficiencylevel-values"></a>Valores skillProficiencyLevel

|Member|
|:---|
|Elementar|
|limitedWorking|
|generalProfessional|
|advancedProfessional|
|Especialista|
|unknownFutureValue|

### <a name="languageproficiencylevel-values"></a>Valores languageProficiencyLevel

|Member|
|:---|
|Elementar|
|Conversação|
|limitedWorking|
|professionalWorking|
|fullProfessional|
|nativeOrBilingual|
|unknownFutureValue|

### <a name="personrelationship-values"></a>valores personRelationship

|Member|
|:---|
|manager|
|Colega|
|directReport|
|dotLineReport|
|Assistente|
|dotLineManager|
|alternateContact|
|Amigo|
|Cônjuge|
|Irmão|
|filho|
|primário|
|Patrocinador|
|emergencyContact|
|Outros|
|unknownFutureValue|

### <a name="attachmenttype-values"></a>Valores attachmentType

| Member
|:--------------
| file
| item
| referência

### <a name="analyticsactivitytype-values"></a>Valores analyticsActivityType

| Member
|:--------------
| call
| chat
| email
| foco
| Reunião

### <a name="registrationauthmethod-values"></a>valores registrationAuthMethod

|Member|
|:---|
|email|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobilePhone|

### <a name="entitytypes-values"></a>Valores entityTypes

|Member|
|:---|
|event|
|message|
|driveItem|
|externalItem|
|site|
|list|
|listItem|
|Unidade|
|unknownFutureValue|

### <a name="searchalterationtype-values"></a>valores searchAlterationType

| Member |
|:---------------|
|Modificação|
|Sugestão|

### <a name="bucketaggregationsortproperty-values"></a>Valores bucketAggregationSortProperty

|Member|
|:---|
|count|
|keyAsString|
|keyAsNumber|

### <a name="contactrelationship-values"></a>valores contactRelationship

| Membro             | Valor | Descrição                              |
| :----------------- | :---- | :--------------------------------------- |
| primário             | 0     | O pai do usuário.                       |
| Relativo           | 1     | O parente do usuário.                     |
| Assessor               | 2     | O assessor do usuário.                         |
| Médico             | 3     | O médico do usuário.                       |
| Guardião           | 4     | O guardião do usuário.                     |
| filho              | 5     | O filho do usuário.                        |
| Outros              | 6      | Uma relação não especificada com o usuário. |
| unknownFutureValue | 7      | Valor do marcador para compatibilidade futura.   |

### <a name="scheduleentitytheme-values"></a>Valores scheduleEntityTheme

| Member
|:-------------------------
| branco
| Azul
| Verde
| Roxo
| Rosa
| Amarelo
| Cinza
| Darkblue
| darkGreen
| darkPurple
| darkPink
| darkYellow
| unknownFutureValue


### <a name="timeoffreasonicontype-values"></a>Valores timeOffReasonIconType

|Member|
|:---|
|none|
|Carro|
|calendar|
|Executando|
|Avião|
|firstAid|
|Médico|
|notWorking|
|Relógio|
|juryDuty|
|Globo|
|Copo|
|phone|
|Tempo|
|Guarda-chuva|
|Piggybank|
|Cão|
|Bolo|
|trafficCone|
|Pino|
|Ensolarado|
|unknownFutureValue|

### <a name="timecardstate-values"></a>Valores de timeCardState

|Member|
|:---|
|clockedIn|
|onBreak|
|clockedOut|
|unknownFutureValue|

### <a name="schedulechangestate-values"></a>Valores de scheduleChangeState

| Member
|:----------------------------
|Pendente
|Aprovado
|Recusou
|unknownFutureValue

### <a name="schedulechangerequestactor-values"></a>Valores de scheduleChangeRequestActor

| Member
|:----------------------------
|remetente
|destinatário
|manager
|sistema
|unknownFutureValue

### <a name="workforceintegrationencryptionprotocol-values"></a>Valores workforceIntegrationEncryptionProtocol

| Member
|:----------------------------
|sharedSecret
|unknownFutureValue

### <a name="workforceintegrationsupportedentities-values"></a>Valores workforceIntegrationSupportedEntities

|Member|
|:---|
|none|
|shift|
|swapRequest|
|userShiftPreferences|
|openShift|
|openShiftRequest|
|offerShiftRequest|
|unknownFutureValue|
|Cartão|
|timeOffReason|
|timeOff|
|timeOffRequest|

### <a name="confirmedby-values"></a>valores confirmedBy

| Member
|:-----------------
| none|
| user|
| manager|
| unknownFutureValue|

### <a name="timezonestandard-values"></a>Valores timeZoneStandard

| Member
|:-----------------
| windows
| Iana


### <a name="freebusystatus-values"></a>Valores freeBusyStatus

| Membro           | Valor |
| :--------------- | :---- |
| Livre             | 0     |
| Provisório        | 1     |
| Ocupado             | 2     |
| Oof              | 3     |
| workingElsewhere | 4     |
| desconhecido          | -1    |


### <a name="physicaladdresstype-values"></a>Valores physicalAddressType

| Member
|:-------------------------
| desconhecido
| Casa
| Negócio
| Outros


### <a name="attendeetype-values"></a>Valores attendeeType

| Member
|:-------------------------
| obrigatório
| opcional
| recurso


### <a name="externalaudiencescope-values"></a>Valores externalAudienceScope

| Member
|:-------------------------
| none
| contactsOnly
| tudo


### <a name="automaticrepliesstatus-values"></a>Valores automaticRepliesStatus

| Member
|:-------------------------
| desabilitadas
| alwaysEnabled
| agendado


### <a name="calendarcolor-values"></a>Valores calendarColor

| Membro      | Valor |
| :---------- | :---- |
| Automático        | -1    |
| Lightblue   | 0     |
| Lightgreen  | 1     |
| lightOrange | 2     |
| Lightgray   | 3     |
| Lightyellow | 4     |
| lightTeal   | 5     |
| Lightpink   | 6      |
| lightBrown  | 7      |
| lightRed    | 8      |
| maxColor    | 9      |


### <a name="educationsynchronizationprofilestate-values"></a>valores educationSynchronizationProfileState

| Membro             | Valor |
| :----------------- | :---- |
| Excluir           | 2     |
| deletionFailed     | 3     |
| provisioningFailed | 5     |
| provisionado        | 6      |
| Provisionamento       | 7      |
| unknownFutureValue | 8      |


### <a name="educationsynchronizationstatus-values"></a>valores educationSynchronizationStatus

| Member             |
| :----------------- |
| Pausado             |
| Inprogress         |
| sucesso            |
| erro              |
| Validationerror    |
| Quarantined        |
| unknownFutureValue |
| Extrair         |
| Validar         |

### <a name="educationexternalsource-values"></a>valores educationExternalSource

| Member
|:-------------------------
| Sis
| Lms
| Manual
| unknownFutureValue

### <a name="educationgender-values"></a>valores educationGender

| Member
|:-------------------------
| Fêmea
| Masculino
| Outros
| unknownFutureValue


### <a name="eventtype-values"></a>valores eventType

| Member
|:-------------------------
| Singleinstance
| Ocorrência
| Exceção
| seriesMaster


### <a name="sensitivity-values"></a>valores de confidencialidade

| Member
|:-------------------------
| Normal
| pessoal
| Privada
| Confidencial


### <a name="importance-values"></a>valores de importância

| Member
|:-------------------------
| low
| Normal
| high


### <a name="educationuserrole-values"></a>valores educationUserRole
| Member
|:---------------------
| student
| teacher
| Faculdade


### <a name="meetingmessagetype-values"></a>Valores meetingMessageType

| Member
|:-----------------
| none
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>Valores followupFlagStatus

| Member
|:-------------------------
| notFlagged
| complete
| Sinalizado


### <a name="inferenceclassificationtype-values"></a>Valores inferenceClassificationType

| Member
|:-----------------
| Focado
| Outros


### <a name="iosnotificationalerttype-values"></a>Valores de iosNotificationAlertType

| Member
|:-------------------------
| deviceDefault
| Banner
| Modal
| none

### <a name="deviceenrollmentfailurereason-values"></a>Valores deviceEnrollmentFailureReason

| Member
|:-------------
| desconhecido
| autenticação
| autorização
| accountValidation
| userValidation
| deviceNotSupported
| inMaintenance
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### <a name="bodytype-values"></a>valores bodyType
| Member
|:---------
| texto
| HTML


### <a name="locationtype-values"></a>valores locationType

| Member
|:-------------------------
| Padrão.
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| Hotel
| Restaurante
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>Valores locationUniqueIdType

| Member
|:-------------------------
| desconhecido
| locationStore
| Diretório
| Privada
| Bing


### <a name="messageactionflag-values"></a>Valores messageActionFlag

| Member
|:-------------------------
| qualquer
| call
| doNotForward
| Continuação
| Fyi
| forward
| noResponseNecessary
| leitura
| reply
| replyToAll
| Revisão


### <a name="onenoteuserrole-values"></a>valores onenoteUserRole

| Membro      | Valor |
| :---------- | :---- |
| Proprietário       | 0     |
| Colaborador | 1     |
| Leitor      | 2     |
| Nenhum        | -1    |


### <a name="operationstatus-values"></a>valores operationStatus

| Member
|:-----------------
|NotStarted
|Em execução
|Concluído
|Falhou


### <a name="onenotepatchactiontype-values"></a>Valores de onenotePatchActionType

| Member
|:-------------------------
| Substituir
| Append
| Excluir
| Inserir
| Preceder

### <a name="onenotepatchinsertposition-values"></a>valores onenotePatchInsertPosition

| Member
|:-------------------------
| After
| Before


### <a name="phonetype-values"></a>Valores phoneType

| Member
|:-------------------------
| Casa
| Negócio
| móvel
| Outros
| Assistente
| homeFax
| businessFax
| Otherfax
| Pager
| Rádio


### <a name="plannerpreviewtype-values"></a>Valores plannerPreviewType

| Member
|:-------------------------
| Automático
| noPreview
| Lista
| descrição
| referência


### <a name="status-values"></a>valores de status

| Member
|:-----------------
| Ativo
| Atualizado
| deleted
| ignorado
| unknownFutureValue


### <a name="weekindex-values"></a>valores weekIndex

| Member
|:-------------------------
| Primeiro
| Segundo
| Terceiro
| Quarto
| Última


### <a name="dayofweek-values"></a>valores dayOfWeek

| Member
|:-------------------------
| Domingo
| Segunda-feira
| Terça
| Quarta
| Quinta
| Sexta
| Sábado

### <a name="recurrencepatterntype-values"></a>Valores recurrencePatternType

| Member
|:-------------------------
| Diária
| Semanal
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>Valores recurrenceRangeType

| Member
|:-------------------------
| endDate
| noEnd
| Numeradas


### <a name="onenotesourceservice-values"></a>valores de onenoteSourceService
| Member
|:---------------------
| Desconhecido
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>valores responseType

| Member
|:-------------------------
| none
| organizer
| tentativelyAccepted
| Aceito
| Recusou
| notResponded


### <a name="activitydomain-values"></a>valores activityDomain

| Member
|:-------------------------
| desconhecido
| trabalho
| pessoal
| irrestrito


### <a name="websitetype-values"></a>valores websiteType

| Member
|:-------------------------
| Outros
| Casa
| trabalho
| blog
| perfil


### <a name="categorycolor-values"></a>valores categoryColor

| Membro   | Valor |
| :------- | :---- |
| none     | -1    |
| preset0  | 0     |
| preset1  | 1     |
| preset2  | 2     |
| preset3  | 3     |
| preset4  | 4     |
| preset5  | 5     |
| preset6  | 6      |
| preset7  | 7      |
| preset8  | 8      |
| preset9  | 9      |
| preset10 | 10    |
| preset11 | 11    |
| preset12 | 12     |
| preset13 | 13    |
| preset14 | 14    |
| preset15 | 15    |
| preset16 | 16    |
| preset17 | 17     |
| preset18 | 18     |
| preset19 | 19    |
| preset20 | 20    |
| preset21 |  21     |
| preset22 | 22    |
| preset23 | 23    |
| preset24 | 24    |

### <a name="alertfeedback-values"></a>valores alertFeedback

Possíveis valores de comentários sobre o alerta fornecido por um analista.

| Membro         | Valor | Descrição               |
| :------------- | :---- | :------------------------ |
| desconhecido        | 0     | Desconhecido.                  |
| truePositive   | 1     | O alerta é verdadeiro positivo.   |
| falsePositive  | 2     | O alerta é falso positivo.  |
| benignPositive | 3     | O alerta é positivo benigno. |

### <a name="filehashtype-values"></a>Valores fileHashType

| Membro              | Valor | Descrição                    |
| :------------------ | :---- | :----------------------------- |
| desconhecido             | 0     | Tipo desconhecido.                  |
| sha1                | 1     | Tipo de hash SHA1.                |
| sha256              | 2     | Tipo de hash SHA256.              |
| md5                 | 3     | Tipo de hash MD5.                 |
| authenticodeHash256 | 4     | Tipo de hash AuthenticodeHash256. |
| lsHash              | 5     | Tipo de hash LsHash.              |
| ctph                | 6      | Tipo de hash CTPH.                |
| peSha1              | 7      | Tipo de hash PESHA1.              |
| peSha256            | 8      | Tipo de hash PESHA256.            |

### <a name="connectiondirection-values"></a>Valores connectionDirection

| Membro   | Valor | Descrição          |
| :------- | :---- | :------------------- |
| desconhecido  | 0     | Conexão desconhecida.  |
| Entrada  | 1     | Conexão de entrada.  |
| Saída | 2     | Conexão de saída. |

### <a name="connectionstatus-values"></a>Valores connectionStatus

| Membro    | Valor | Descrição                |
| :-------- | :---- | :------------------------- |
| desconhecido   | 0     | Status de conexão desconhecido. |
| Tentativa | 1     | Tentativa de conexão.      |
| Conseguiu | 2     | Conexão bem-sucedida.      |
| Bloqueado   | 3     | Conexão bloqueada.        |
| Falhou    | 4     | Falha na conexão.         |

### <a name="processintegritylevel-values"></a>Valores processIntegrityLevel

| Membro    | Valor | Descrição                   |
| :-------- | :---- | :---------------------------- |
| desconhecido   | 0     | Desconhecido.                      |
| Untrusted | 10    | O nível de integridade não é confiável. |
| low       | 20    | O nível de integridade é Baixo.       |
| medium    | 30    | O nível de integridade é Médio.    |
| high      | 40    | O nível de integridade é Alto.      |
| sistema    | 50    | O nível de integridade é System.    |

### <a name="registryhive-values"></a>valores registryHive

Enumeração para hives do Registro conforme definido pelos [Hives do Registro](/windows/desktop/sysinfo/registry-hives).

| Membro                  | Valor | Descrição                       |
| :---------------------- | :---- | :-------------------------------- |
| desconhecido                 | 0     | Hive desconhecido.                     |
| Currentconfig           | 1     | HKEY_CURRENT_CONFIG hive.         |
| Currentuser             | 2     | HKEY_CURRENT_USER hive.           |
| localMachineSam         | 3     | HKEY_LOCAL_MACHINE\SAM hive.      |
| localMachineSamSoftware | 4     | HKEY_LOCAL_MACHINE\Software hive. |
| localMachineSystem      | 5     | HKEY_LOCAL_MACHINE\System hive.   |
| usersDefault            | 6      | \\HKEY_USERS. Hive PADRÃO.        |

### <a name="registryoperation-values"></a>valores de registryOperation

Operação que alterou o nome e/ou o valor da chave do Registro.

| Membro  | Valor | Descrição                  |
| :------ | :---- | :--------------------------- |
| desconhecido | 0     | Tipo de valor de registro desconhecido. |
| create  | 1     | Criar registro.             |
| Modificar  | 2     | Modifique o registro.             |
| delete  | 3     | Excluir registro.             |

### <a name="registryvaluetype-values"></a>Valores registryValueType

Enumeração para tipos de valor do Registro conforme definido pelos [tipos de valor do Registro](/windows/desktop/sysinfo/registry-value-types).

| Membro            | Valor | Descrição                                  |
| :---------------- | :---- | :------------------------------------------- |
| desconhecido           | 0     | Tipo de valor de registro desconhecido.                 |
| Binário            | 1     | REG_BINARY tipo de valor do Registro.              |
| Dword             | 2     | REG_DWORD tipo de valor do Registro.               |
| dwordWordScriptEndian | 3     | REG_DWORD_LITTLE_ENDIAN tipo de valor do Registro. |
| dwordBigEndian    | 4     | REG_DWORD_BIG_ENDIAN tipo de valor do Registro.    |
| expandSz          | 5     | REG_EXPAND_SZ tipo de valor do Registro.           |
| link              | 6      | REG_LINK tipo de valor do Registro.                |
| multiSz           | 7      | REG_MULTI_SZ tipo de valor do Registro.            |
| none              | 8      | REG_NONE tipo de valor do Registro.                |
| Qword             | 9      | REG_QWORD tipo de valor do Registro.               |
| qwordwordEndian | 10    | REG_QWORD_LITTLE_ENDIAN tipo de valor do Registro. |
| Sz                | 11    | REG_SZ tipo de valor do Registro.                  |

### <a name="alertseverity-values"></a>Valores alertSeverity

Enumeração de severidade de alertas.

| Membro        | Valor | Descrição                       |
| :------------ | :---- | :-------------------------------- |
| desconhecido       | 0     | A gravidade é desconhecida.              |
| Informativo | 1     | A severidade é apenas para informações. |
| low           | 2     | A gravidade é baixa.                  |
| medium        | 3     | A gravidade é média.               |
| high          | 4     | A gravidade é alta.                 |

### <a name="alertstatus-values"></a>valores alertStatus

Valores possíveis de um status de ciclo de vida de alerta (estágio).

| Membro     | Valor | Descrição           |
| :--------- | :---- | :-------------------- |
| desconhecido    | 0     | Status desconhecido.       |
| newAlert   | 10    | O alerta é novo.         |
| Inprogress | 20    | O alerta está em andamento. |
| resolvido   | 30    | O alerta é resolvido.    |

### <a name="emailrole-values"></a>Valores de emailRole

Valores possíveis para funções de email.

| Membro    | Valor | Descrição             |
| :-------- | :---- | :---------------------- |
| desconhecido   | 0     | Função Desconhecida.           |
| sender    | 1     | Remetente do email.    |
| destinatário | 2     | Destinatário do email. |

### <a name="logontype-values"></a>valores logonType

Valores possíveis para o método de entrada do usuário.

| Membro            | Valor | Descrição                  |
| :---------------- | :---- | :--------------------------- |
| desconhecido           | -1    | Desconhecido.                     |
| Interativo       | 0     | O logon é interativo.        |
| remoteInteractive | 1     | O logon é interativo remoto. |
| Rede           | 2     | Logon é rede.            |
| batch             | 3     | Logon é lote.              |
| serviço           | 4     | Logon é serviço.            |

### <a name="useraccountsecuritytype-values"></a>Valores userAccountSecurityType

Valores possíveis para tipos de conta de usuário (associação de grupo), de acordo com a definição do Windows.

| Membro        | Valor | Descrição                     |
| :------------ | :---- | :------------------------------ |
| desconhecido       | -1    | Desconhecido.                        |
| padrão      | 0     | Membro do grupo Usuários Padrão. |
| Poder         | 1     | Membro do grupo Usuários Avançados.    |
| Administrador | 2     | Membro do grupo Administradores. |

### <a name="chatmessagepolicyviolationdlpactiontype-values"></a>Valores chatMessagePolicyViolationDlpActionType

| Valor |
|:-----------------|
| none |
| NotifySender |
| BlockAccess |
| BlockAccessExternal |

### <a name="scopeoperatormultivaluedcomparisontype-values"></a>Valores scopeOperatorMultiValuedComparisonType

|Member|
|:---|
|tudo|
|qualquer|

### <a name="risklevel-values"></a>valores riskLevel

|Member|
|:---|
|low|
|medium|
|high|
|hidden|
|none|
|unknownFutureValue|

### <a name="riskstate-values"></a>Valores riskState

|Member|
|:---|
|none|
|confirmedSafe|
|corrigido|
|Demitido|
|atRisk|
|confirmedCompromised|
|unknownFutureValue|

### <a name="advancedconfigstate-values"></a>valores advancedConfigState

|Member|
|:---|
|Padrão.|
|habilitadas|
|desabilitadas|
|unknownFutureValue|

### <a name="referenceattachmentpermission-values"></a>Valores referenceAttachmentPermission

|Member|
|:---|
|Outros|
|modo de exibição|
|edit|
|anonymousView|
|anonymousEdit|
|organizationView|
|organizationEdit|

### <a name="referenceattachmentprovider-values"></a>Valores referenceAttachmentProvider

|Member|
|:---|
|Outros|
|oneDriveBusiness|
|oneDriveConsumer|
|Dropbox|

### <a name="networktype-values"></a>valores networkType

|Member|
|:---|
|Intranet|
|Extranet|
|namedNetwork|
|Confiável|
|unknownFutureValue|

### <a name="exchangeidformat-values"></a>Valores de exchangeIdFormat

|Member|
|:---|
|Entryid|
|ewsId|
|immutableEntryId|
|restId|
|restImmutableEntryId|

### <a name="attributeflowbehavior-values"></a>Valores attributeFlowBehavior

|Member|
|:---|
|flowWhenChanged|
|flowAlways|

### <a name="attributeflowtype-values"></a>Valores attributeFlowType

|Member|
|:---|
|Sempre|
|objectAddOnly|
|multiValueAddOnly|
|restId|

### <a name="objectflowtypes-values"></a>Valores de objectFlowTypes

| Membro | Valor |
| :----- | :---- |
| Nenhuma   | 0     |
| Adicionar    | 1     |
| Atualizar | 2     |
| Excluir | 4     |

### <a name="chatmessagetype-values"></a>Valores chatMessageType

|Member|
|:---|
|message|
|chatEvent |
|Digitação |
|unknownFutureValue|
|systemEventMessage|

### <a name="chatmessageimportance-values"></a>Valores de chatMessageImportance

|Member|
|:---|
|Normal|
|high|
|Urgente|

### <a name="channelmembershiptype-values"></a>Valores channelMembershipType

| Member             |
| :----------------- |
| padrão           |
| Privada            |
| unknownFutureValue |
| compartilhado             |

### <a name="stagedfeaturename-values"></a>Valores stagedFeatureName

| Member                    | Descrição                   |
| :------------------------ | :---------------------------- |
| passthroughAuthentication | Autenticação de passagem    |
| seamlessSso               | Logon Único Contínuo       |
| passwordHashSync          | Sincronização de hash de senha |
| emailAsAlternateId        | Email como uma ID alternativa      |
| unknownFutureValue        | Um membro do Sentinel             |

### <a name="tokenissuertype-values"></a>Valores tokenIssuerType

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|unknownFutureValue|
|AzureADBackupAuth|
|ADFederationServicesMFAAdapter|
|NPSExtension|


### <a name="riskdetectiontimingtype-values"></a>Valores riskDetectionTimingType

|Member|
|:---|
|notDefined|
|Realtime|
|nearRealtime|
|Offline|
|unknownFutureValue|

### <a name="activitytype-values"></a>Valores activityType

|Member|
|:---|
|Signin|
|user|
|unknownFutureValue|
|servicePrincipal|

### <a name="chatmessagepolicyviolationuseractiontype-values"></a>Valores chatMessagePolicyViolationUserActionType

| Member   | Valor int |  Descrição |
|:---------------|:--------|:----------|
| Nenhum | 0 | Valor padrão. Esse é o valor em uma mensagem quando o usuário não executa uma ação na mensagem bloqueada pela DLP. |
| Override | 1 | O remetente substituiu o veredicto da mensagem e enviou a mensagem mesmo assim.|
| ReportFalsePositive | 2 | O remetente relatou o veredicto da mensagem aos administradores como um falso positivo.|

### <a name="chatmessagepolicyviolationverdictdetailstype-values"></a>Valores chatMessagePolicyViolationVerdictDetailsType

| Member   | Valor int |  Descrição |
|:---------------|:--------|:----------|
| Nenhum | 0 |  O usuário não tem permissão para substituir a mensagem. O usuário não tem permissão para relatar uma mensagem como falso positivo se a dica de política não for fornecida. Em todos os outros cenários, o usuário pode relatar uma mensagem como falso positivo.|
| AllowFalsePositiveOverride | 1 |  O usuário não tem permissão para substituir explicitamente o bloco, a menos que isso seja combinado com `AllowOverrideWithoutJustification` ou `AllowOverrideWithJustification` sinalizadores. Relatar um falso positivo na violação substitui automaticamente o bloco e envia a mensagem. |
| AllowOverrideWithoutJustification | 2 | O usuário tem permissão para substituir o bloco e enviar a mensagem. O texto de justificativa não é necessário. Exclusivo para `AllowOverrideWithJustification`. |
| AllowOverrideWithJustification | 4 |  O usuário tem permissão para substituir o bloco e enviar a mensagem. O texto de justificativa é necessário. Exclusivo para `AllowOverrideWithoutJustification`.|

### <a name="entitytype-values"></a>valores entityType

| Member       |
|:--------------|
|event|
|message|
|driveItem|
|externalFile|
|externalItem|

### <a name="onlinemeetingprovidertype-values"></a>Valores onlineMeetingProviderType

|Member|
|:---|
|desconhecido|
|skypeForBusiness|
|skypeForConsumer|
|teamsForBusiness|

### <a name="delegatemeetingmessagedeliveryoptions-values"></a>Valores delegateMeetingMessageDeliveryOptions

|Member|
|:---|
|sendToDelegateAndInformationToPrincipal|
|sendToDelegateAndPrincipal|
|sendToDelegateOnly|

### <a name="calendarroletype-values"></a>Valores calendarRoleType

|Member|
|:---|
|none|
|freeBusyRead|
|limitedRead|
|leitura|
|gravação|
|delegateWithoutPrivateEventAccess|
|delegateWithPrivateEventAccess|
|Personalizado|

### <a name="contentformat-values"></a>Valores contentFormat

| Membro  | Valor | Descrição                          |
| :------ | :---- | :----------------------------------- |
| Padrão. | 0     | O conteúdo é um arquivo ou um tipo que não é de email. |
| email   | 1     | O conteúdo é um email.                 |

### <a name="contentstate-values"></a>Valores contentState

| Membro | Valor | Descrição                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| Resto   | 0     | Os dados estão em repouso; Um arquivo em um compartilhamento, por exemplo.                                 |
| Movimento | 1     | Os dados estão em movimento. Um arquivo interceptado por um dispositivo de rede em trânsito.         |
| Usar    | 2     | Os dados estão em uso. Um arquivo é aberto em um aplicativo cliente, como o Microsoft Office. |

### <a name="assignmentmethod-values"></a>Valores assignmentMethod

| Membro     | Valor | Descrição                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| padrão   | 0     | O rótulo foi definido por uma condição de serviço ou política.                                                                              |
| Privilegiada | 1     | O rótulo foi definido explicitamente por um usuário.                                                                                          |
| Automático       | 2     | Permite a substituição de qualquer rótulo existente. Justificativa necessária no downgrade. Resulta no método `standard` de atribuição em metadados. |

### <a name="actionsource-values"></a>valores actionSource

| Membro        | Valor | Descrição                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| Manual        | 0     | Um usuário selecionou manualmente o rótulo.                          |
| Automático     | 1     | O rótulo foi escolhido como resultado das condições da política.       |
| recomendado   | 2     | O escolhido para aplicar um rótulo recomendado.                    |
| policyDefault | 3     | O usuário não tem nenhuma ação e o rótulo padrão de política foi aplicado. |
| Obrigatório     | 4     | O usuário escolheu um rótulo depois de ser forçado a escolher.         |

### <a name="contentalignment-values"></a>Valores contentAlignment

| Membro | Valor | Descrição                         |
| :----- | :---- | :---------------------------------- |
| left   | 0     | Alinhe a marcação de conteúdo à esquerda.  |
| Certo  | 1     | Alinhe a marcação de conteúdo à direita. |
| Centro | 2     | Centralizar a marcação de conteúdo.             |

### <a name="watermarklayout-values"></a>Valores watermarkLayout

| Membro     | Valor | Descrição                 |
| :--------- | :---- | :-------------------------- |
| Horizontal | 0     | Use uma marca d'água horizontal. |
| Diagonal   | 1     | Use uma marca d'água diagonal.   |

### <a name="conditionalaccesspolicystate-values"></a>Valores conditionalAccessPolicyState

|Member|
|:---|
|habilitadas|
|desabilitadas|
|enabledForReportingButNotEnforced|

### <a name="conditionalaccessgrantcontrol-values"></a>Valores conditionalAccessGrantControl

| Member       |
|:--------------|
|Bloco|
|Amf|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|
|passwordChange|
|unknownFutureValue|

### <a name="conditionalaccessrule-values"></a>Valores conditionalAccessRule 

|Member|
|:---|
|allApps|
|firstPartyApps|
|office365|
|appId|
|Acr|
|appFilter|
|Allusers|
|Convidado|
|groupId|
|roleId|
|userId|
|allDevicePlatforms|
|devicePlatform|
|allLocations|
|insideCorpnet|
|allTrustedLocations|
|Locationid|
|allDevices|
|deviceFilter|
|deviceState|
|unknownFutureValue|
|deviceFilterIncludeRuleNotMatched|
|allDeviceStates|
|anonymizedIPAddress|
|unfamiliarFeatures|
|nationStateIPAddress|
|realTimeThreatIntelligence|
|internalGuest|
|b2bCollaborationGuest|
|b2bCollaborationMember|
|b2bDirectConnectUser|
|otherExternalUser|
|Serviceprovider|

### <a name="signinaccesstype-values"></a>Valores signInAccessType 

|Member|
|:---|
|none|
|b2bCollaboration|
|b2bDirectConnect|
|microsoftSupport|
|Serviceprovider|
|unknownFutureValue|

### <a name="signinfrequencytype-values"></a>Valores signinFrequencyType

| Member       |
|:--------------|
|Dias|
|Horas|

### <a name="persistentbrowsersessionmode-values"></a>Valores persistentBrowserSessionMode

| Member       |
|:--------------|
|Sempre|
|Nunca|

### <a name="cloudappsecuritysessioncontroltype-values"></a>Valores cloudAppSecuritySessionControlType

| Member       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|

### <a name="conditionalaccessdeviceplatform-values"></a>Valores conditionalAccessDevicePlatform

| Member       |
|:--------------|
|Android|
|iOS|
|windows|
|windowsPhone|
|macOS|
|tudo|
|unknownFutureValue|

### <a name="priority-values"></a>valores de prioridade

|Membro|Valor|
|:---|:---|
|Nenhuma|0|
|Alta|1|
|Baixo|2|

### <a name="threatassessmentcontenttype-values"></a>Valores threatAssessmentContentType

| Membro | Valor | Descrição             |
|:-------|:------|:------------------------|
| email   | 1     | Ameaça de email.            |
| url    | 2     | Ameaça de URL.             |
| file   | 3     | Ameaça de arquivo de anexo. |

### <a name="threatexpectedassessment-values"></a>Valores threatExpectedAssessment

| Membro  | Valor | Descrição                       |
|:--------|:------|:----------------------------------|
| Bloco   | 1     | A ameaça deve ser bloqueada.     |
| Desbloquear | 2     | A ameaça não deve ser bloqueada. |

### <a name="threatcategory-values"></a>Valores threatCategory

| Membro             | Valor | Descrição        |
|:-------------------|:------|:-------------------|
| spam               | 1     | Ameaça de spam.       |
| phishing           | 2     | Ameaça de phishing.   |
| malware            | 3     | Ameaça de malware.    |
| unknownFutureValue | 4     | Um membro do Sentinel. |

### <a name="threatassessmentstatus-values"></a>Valores threatAssessmentStatus

| Membro    | Valor | Descrição                              |
|:----------|:------|:-----------------------------------------|
| Pendente   | 1     | A avaliação de ameaças ainda está em andamento. |
| Concluído | 2     | A avaliação de ameaças foi concluída.         |

### <a name="threatassessmentrequestsource-values"></a>Valores threatAssessmentRequestSource

| Membro        | Valor | Descrição              |
|:--------------|:------|:-------------------------|
| Indefinido     | 0     | Ainda não sei.            |
| user          | 1     | Envio do usuário.         |
| Administrador | 2     | Envio de administrador de locatários. |

### <a name="threatassessmentresulttype-values"></a>Valores threatAssessmentResultType

| Membro             | Valor | Descrição                                          |
|:-------------------|:------|:-----------------------------------------------------|
| Checkpolicy        | 1     | O resultado da verificação de política, somente para `mail` avaliação. |
| Rescan             | 2     | O resultado da nova verificação.                                   |
| unknownFutureValue | 3     | Um membro do Sentinel.                                   |

### <a name="maildestinationroutingreason-values"></a>Valores mailDestinationRoutingReason

| Membro                | Valor | Descrição                         |
|:----------------------|:------|:------------------------------------|
| none                  | 0     | Ainda não sei.                       |
| mailFlowRule          | 1     | Regra de transporte do Exchange.            |
| safeSender            | 2     | Lista de remetentes seguros.                   |
| blockedSender         | 3     | Lista de remetentes bloqueados.                |
| advancedSpamFiltering | 4     | Opção avançada de filtragem de spam.     |
| domainAllowList       | 5     | Lista de permissões de domínio do remetente.           |
| domainBlockList       | 6      | Lista de bloqueios de domínio do remetente.           |
| notInAddressBook      | 7      | Exclua o remetente que não está no catálogo de endereços. |
| firstTimeSender       | 8      | Bloqueado devido ao remetente da primeira vez.   |
| autoPurgeToInbox      | 9      | TimeTravel move a mensagem para a caixa de entrada.   |
| autoPurgeToJunk       | 10    | TimeTravel move mensagem para lixo eletrônico.    |
| autoPurgeToDeleted    | 11    | Mensagem de movimentação timeTravel a ser excluída. |
| Saída              | 12     | Email de saída.                      |
| notJunk               | 13    | Permita devido a não lixo eletrônico.              |
| Lixo                  | 14    | Bloqueado devido a lixo eletrônico.                |
| unknownFutureValue    | 15    | Um membro do Sentinel.                  |

### <a name="threatassessmentrequestpivotproperty-values"></a>Valores threatAssessmentRequestPivotProperty

| Membro                       | Valor | Descrição                                                            |
|:-----------------------------|:------|:-----------------------------------------------------------------------|
| threatCategory               | 1     | Agregação de solicitação de avaliação de ameaças por `threatCategory`.               |
| mailDestinationRoutingReason | 2     | Agregação de solicitação de avaliação de ameaças por `mailDestinationRoutingReason`. |

### <a name="userflowtype-values"></a>Valores userFlowType

|Member
|:----------------------
| Inscrição
| Signin
| signUpOrSignIn
| passwordReset
| profileUpdate
| resourceOwner
| unknownFutureValue

### <a name="openidconnectresponsemode-values"></a>Valores de openIdConnectResponseMode

| Member
|:----------------------
| form_post
| consulta
| unknownFutureValue

### <a name="wellknownlistname-values"></a>Valores wellknownListName

| Member
|:----------------------
| none
| defaultList
| flaggedEmails
| unknownFutureValue

### <a name="taskstatus-values"></a>Valores taskStatus

| Member
|:----------------------
| Notstarted
| Inprogress
| Concluído
| waitingOnOthers
| Adiada

### <a name="columntypes-values"></a>Valores columnTypes

|Member|Descrição|
|:-------|:------
|Nota| texto multilinha. |
|texto | texto de linha única. |
|Escolha | coluna de escolha |
|Multichoice | coluna multichoice. |
|number | coluna de número. |
|Moeda | coluna de moeda. |
|dateTime | Coluna dateTime. |
|Pesquisa | coluna de pesquisa. |
|booliano | Coluna Sim/Não. |
|user | coluna de pessoa ou grupo. |
|url | hiperlink ou coluna de imagem. |
|Calculado | coluna calculada. |
|localização | coluna de localização. |
|Localização geográfica | coluna de localização geográfica. |
|term | coluna de metadados gerenciados. |
|Multiterm | coluna de metadados gerenciados aceitando vários valores. |
|Miniatura | Coluna de imagem. |
|Approvalstatus | Coluna de status de aprovação de conteúdo. |
|unknownFutureValue | unknownFuturevalue |

### <a name="connectedorganizationstate-values"></a>Valores connectedOrganizationState

| Membro                | Valor | Descrição                                                                                                                                                                                                        |
|:----------------------| :-----|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Configurado            | 0     | As organizações conectadas com esse valor de estado são incluídas nas políticas de atribuição com o tipo de escopo do solicitante `AllConfiguredConnectedOrganizationSubjects`.                                                          |
| Proposta              | 1     | As organizações conectadas que são criadas automaticamente pelo sistema têm esse valor de estado. Eles não são incluídos em políticas de atribuição com o tipo de escopo do solicitante `AllConfiguredConnectedOrganizationSubjects`.   |
| unknownFutureValue    | 2     | Um membro do Sentinel.                                                                                                                                                                                                 |

### <a name="identityuserflowattributedatatype-values"></a>Valores identityUserFlowAttributeDataType

| Membro                | Valor | Descrição                         |
|:----------------------|:------|:------------------------------------|
| string                | 1     | Tipo de dados de cadeias de caracteres                    |
| booliano               | 2     | Tipo de dados Booliano                   |
| int64                 | 3     | Tipo de dados Int                       |
| Stringcollection      | 4     | Tipo de dados de coleção de cadeias de caracteres         |
|dateTime|5||
| unknownFutureValue    | 6      | Um membro do Sentinel.                  |

### <a name="identityuserflowattributetype-values"></a>Valores identityUserFlowAttributeType

| Membro                | Valor | Descrição                                                        |
|:----------------------|:------|:-------------------------------------------------------------------|
| Builtin               | 1     | Esse tipo de atributo de fluxo de usuário indica que ele foi criado pelo sistema |
| Personalizado                | 2     | Esse tipo de atributo de fluxo de usuário indica que ele foi criado pelo usuário   |
|obrigatório|3||
| unknownFutureValue    | 4     | Um membro do Sentinel.                                                 |

### <a name="permissionclassificationtype-values"></a>Valores permissionClassificationType

| Member
|:-------
| low

### <a name="permissiontype-values"></a>Valores permissionType

| Member
|:-------------------------
| aplicação
| Delegada
| delegatedUserConsentable

### <a name="identityuserflowattributeinputtype-values"></a>Valores identityUserFlowAttributeInputType

| Member                |
|:----------------------|
| Textbox               |
| dateTimeDropDown      |
| radioSingleSelect     |
| dropdownSingleSelect  |
| emailBox              |
| checkboxMultiSelect   |

### <a name="teamworkactivitytopicsource-values"></a>Valores de teamworkActivityTopicSource

| Member
|:---
| entityUrl
| texto

### <a name="cloudpcprovisioningpolicyimagetype-values"></a>Valores cloudPcProvisioningPolicyImageType

|Member|
|:---|
|Personalizado|
|Galeria|

### <a name="chattype-values"></a>Valores chatType

| Membro             | Valor | Descrição               |
| :----------------- | :---- | :------------------------ |
|oneOnOne            | 0     | Indica que o chat é um chat 1:1. O tamanho da lista de participantes é fixo para esse tipo de chat, o membro não pode ser removido/adicionado.                  |
|group               | 1     | Indica que o chat é um chat em grupo. O tamanho da lista de participação (de pelo menos 2 pessoas) pode ser atualizado para esse tipo de chat. Os membros podem ser removidos/adicionados posteriormente.   |
|Reunião             | 2     | Indica que o chat é um chat de reunião, que é criado como um efeito colateral da criação de um OnlineMeeting.  |
|unknownFutureValue  | 3     | Valor do Sentinel para indicar valores futuros. |

### <a name="singlesignonmode-values"></a>valores singleSignOnMode

|Member|
|:---|
|none|
|onPremisesKerberos|
|aadHeaderBased|
|pingHeaderBased|

### <a name="plannercontainertype-values"></a>Valores plannerContainerType

|Member|
|:---|
|group|
|unknownFutureValue|
|lista de participantes|

### <a name="plannerplancontexttype-values"></a>Valores plannerPlanContextType

|Member|
|:---|
|teamsTab|
|sharePointPage|
|meetingNotes|
|Outros|
|unknownFutureValue|

### <a name="plannercontextstate-values"></a>Valores de plannerContextState

|Member             |
|:------------------|
|Ativo             |
|desvinculado           |
|unknownFutureValue |  


### <a name="policyscope-values"></a>Valores de policyScope

|Member|
|:---|
|none|
|tudo|
|Selecionado|

### <a name="teamsappinstallationscope-values"></a>Valores de teamsAppInstallationScope

|Membro    |Valor    |Descrição |
|:---------|:--------|:----------- |
|team      |0        |Indica que o aplicativo Teams pode ser instalado em uma equipe e está autorizado a acessar os dados dessa equipe.|
|Groupchat |1        |Indica que o aplicativo Teams pode ser instalado em um chat em grupo e está autorizado a acessar os dados desse chat em grupo.|
|pessoal  |2        |Indica que o aplicativo Teams pode ser instalado no escopo pessoal de um usuário e está autorizado a acessar os dados desse usuário.|

### <a name="roleassignmentschedulerequestfilterbycurrentuseroptions-values"></a>Valores roleAssignmentScheduleRequestFilterByCurrentUserOptions

|Member|
|:---|
|principal|
|createdBy|
|Aprovador|
|unknownFutureValue|

### <a name="roleassignmentschedulefilterbycurrentuseroptions-values"></a>Valores roleAssignmentScheduleFilterByCurrentUserOptions

|Member|
|:---|
|principal|
|unknownFutureValue|

### <a name="roleassignmentscheduleinstancefilterbycurrentuseroptions-values"></a>Valores roleAssignmentScheduleInstanceFilterByCurrentUserOptions

|Member|
|:---|
|principal|
|unknownFutureValue|

### <a name="roleeligibilityschedulerequestfilterbycurrentuseroptions-values"></a>Valores roleEligibilityScheduleRequestFilterByCurrentUserOptions

|Member|
|:---|
|principal|
|createdBy|
|Aprovador|
|unknownFutureValue|

### <a name="roleeligibilityschedulefilterbycurrentuseroptions-values"></a>Valores roleEligibilityScheduleFilterByCurrentUserOptions

|Member|
|:---|
|principal|
|unknownFutureValue|

### <a name="roleeligibilityscheduleinstancefilterbycurrentuseroptions-values"></a>Valores roleEligibilityScheduleInstanceFilterByCurrentUserOptions

|Member|
|:---|
|principal|
|unknownFutureValue|

### <a name="cloudpcauditactivityoperationtype-values"></a>Valores cloudPcAuditActivityOperationType

|Member|
|:---|
|create|
|delete|
|Patch|
|Outros|

### <a name="cloudpcauditactivityresult-values"></a>Valores de cloudPcAuditActivityResult

|Member|
|:---|
|sucesso|
|clientError|
|Falha|
|timeout|
|Outros|

### <a name="cloudpcauditactortype-values"></a>Valores cloudPcAuditActorType

|Member|
|:---|
|Itpro|
|aplicação|
|Parceiro|
|desconhecido|

### <a name="cloudpcauditcategory-values"></a>Valores cloudPcAuditCategory

|Member|
|:---|
|cloudPC|
|Outros|

### <a name="posttype-values"></a>Valores postType

|Member|
|:---|
|Regular|
|Rápido|
|Estratégico|
|unknownFutureValue|

### <a name="servicehealthclassificationtype-values"></a>Valores serviceHealthClassificationType

|Member|
|:---|
|Consultivo|
|Incidente|
|unknownFutureValue|

### <a name="servicehealthorigin-values"></a>Valores serviceHealthOrigin

|Member|
|:---|
|microsoft|
|thirdParty|
|Cliente|
|unknownFutureValue|

### <a name="servicehealthstatus-values"></a>Valores serviceHealthStatus

|Member|
|:---|
|serviceOperational|
|investigar|
|restoringService|
|verifyingService|
|serviceRestored|
|postIncidentReviewPublished|
|serviceDegradation|
|serviceInterruption|
|extendedRecovery|
|falsePositive|
|investigationSuspended|
|resolvido|
|mitigatedExternal|
|Atenuado|
|resolvedExternal|
|Confirmou|
|Relatado|
|unknownFutureValue|

### <a name="serviceupdatecategory-values"></a>Valores serviceUpdateCategory

|Member|
|:---|
|preventOrFixIssue|
|planForChange|
|stayInformed|
|unknownFutureValue|

### <a name="serviceupdateseverity-values"></a>Valores serviceUpdateSeverity

|Member|
|:---|
|Normal|
|high|
|Crítico|
|unknownFutureValue|

### <a name="teamworktagtype-values"></a>Valores teamworkTagType

|Membro| Valor | Descrição               |
|:---|:---- | :------------------------ |
|padrão| 0     |Tipo padrão para uma marca. As marcas do tipo padrão podem ser gerenciadas na equipe por membros que têm permissões.|

### <a name="teamworkapplicationidentitytype-values"></a>Valores teamworkApplicationIdentityType

|Member|
|:---|
|aadApplication|
|bot|
|tenantBot|
|office365Connector|
|outgoingWebhook|
|unknownFutureValue|

### <a name="teamworkconversationidentitytype-values"></a>Valores teamworkConversationIdentityType

|Member|
|:---|
|team|
|Canal|
|chat|
|unknownFutureValue|

### <a name="teamworkuseridentitytype-values"></a>Valores teamworkUserIdentityType

|Member|
|:---|
|aadUser|
|onPremiseAadUser|
|anonymousGuest|
|federatedUser|
|personalMicrosoftAccountUser|
|skypeUser|
|phoneUser|
|unknownFutureValue|
|emailUser|

### <a name="callrecordingstatus-values"></a>valores callRecordingStatus

|Member|
|:---|
|sucesso|
|Falha|
|Inicial|
|chunkFinished|
|unknownFutureValue|

### <a name="payloaddeliveryplatform-values"></a>valores payloadDeliveryPlatform

|Member|
|:---|
|desconhecido|
|Sms|
|email|
|Equipes|
|unknownFutureValue|

### <a name="trainingstatus-values"></a>valores trainingStatus

|Member|
|:---|
|desconhecido|
|Atribuído|
|Inprogress|
|Concluído|
|Atrasada|
|unknownFutureValue|

### <a name="teamworkcalleventtype-values"></a>Valores teamworkCallEventType

|Member|
|:---|
|call|
|Reunião|
|screenShare|
|unknownFutureValue|

### <a name="binaryoperator-values"></a>Valores binaryOperator 

|Member|
|:---|
|ou|
|e|

### <a name="subjectrightsrequeststage-values"></a>valores subjectRightsRequestStage 

|Member|
|:---|
|contentRetrieval|
|contentReview| 
|generateReport| 
|contentDeletion|
|caseResolved|
|unknownFutureValue|

### <a name="subjectrightsrequeststagestatus-values"></a>valores subjectRightsRequestStageStatus 

|Member|
|:---|
|Notstarted|
|Atual|
|Concluído|
|Falhou|
|unknownFutureValue|

### <a name="subjectrightsrequeststatus-values"></a>Valores subjectRightsRequestStatus 

|Member|
|:---|
|Ativo|
|Fechado|
|unknownFutureValue|

### <a name="subjectrightsrequesttype-values"></a>Valores subjectRightsRequestType 

|Member|
|:---|
|Exportação|
|delete|
|Acesso|
|tagForAction|
|unknownFutureValue|

### <a name="datasubjecttype-values"></a>Valores dataSubjectType 

|Member|
|:---|
|Cliente|
|currentEmployee|
|formerEmployee|
|prospectiveEmployee|
|student|
|teacher|
|Faculdade|
|Outros|
|unknownFutureValue|

### <a name="answerinputtype-values"></a>Valores answerInputType

|Membro|Valor|Descrição|
|:---|:---|:---|
|texto|0|Texto.|
|Radiobutton|1|Radiobutton.|
|unknownFutureValue|2|UnknownFutureValue.|

### <a name="taskstatus_v2-values"></a>taskStatus_v2 valores

|Member|
|:---|
|Notstarted|
|Inprogress|
|Concluído|
|unknownFutureValue|


### <a name="wellknownlistname_v2-values"></a>wellKnownListName_v2 valores

|Member|
|:---|
|none|
|defaultList|
|flaggedEmail|
|unknownFutureValue|

### <a name="bookingpricetype-values"></a>valores bookingPriceType

|Member|
|:---|
|Indefinido|
|fixedPrice|
|startingAt|
|Horária|
|Livre|
|priceVaries|
|Calo|
|Notset|
|unknownFutureValue|

### <a name="bookingstaffrole-values"></a>Valores bookingStaffRole 

|Member|
|:---|
|Convidado|
|Administrador|
|Visualizador|
|externalGuest|
|unknownFutureValue|
|Agendador|
|Membro|

### <a name="bookingreminderrecipients-values"></a>valores bookingReminderRecipients 

|Member|
|:---|
|allAttendees|
|Pessoal|
|Cliente|
|unknownFutureValue|

### <a name="teamworkconnectionstatus-values"></a>Valores teamworkConnectionStatus

| Member |
|:--------|
|desconhecido|
|Conectado|
|Desconectado|
|unknownFutureValue|

### <a name="teamworkdeviceactivitystate-values"></a>Valores teamworkDeviceActivityState

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|desconhecido|0|Estado desconhecido.|
|Ocupado|1|O dispositivo está ocupado.|
|Ocioso|2|O dispositivo está ocioso.|
|Indisponível|3|O dispositivo não está disponível.|
|unknownFutureValue|4|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="teamworkdeviceoperationtype-values"></a>Valores teamworkDeviceOperationType

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|deviceRestart|0|Reinicie um dispositivo.|
|configUpdate|1|Atualize a configuração do dispositivo.|
|deviceDiagnostics|2|Obtenha os logs do dispositivo.|
|softwareUpdate|3|Atualize um software no dispositivo.|
|deviceManagementAgentConfigUpdate|4|Atualize a configuração do agente do dispositivo.|
|remoteLogin|5|Logon remoto do dispositivo.|
|remoteLogout|6 |Logoff remoto do dispositivo.|
|unknownFutureValue|7 |Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="teamworksoftwarefreshness-values"></a>Valores teamworkSoftwareFreshness

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|desconhecido|0|Valor desconhecido.|
|Últimas|1|Indica se um componente de dispositivo executa a versão mais recente do software.|
|Updateavailable|2|Indica que uma atualização de software está disponível para um componente de dispositivo.|
|unknownFutureValue|3|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="teamworksoftwaretype-values"></a>Valores teamworkSoftwareType

| Member |
|:---------------|
|adminAgent|
|operatingSystem|
|teamsClient|
|Firmware|
|partnerAgent|
|companyPortal|
|unknownFutureValue|

### <a name="teamworksupportedclient-values"></a>Valores teamworkSupportedClient

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|desconhecido|0|Valor desconhecido.|
|skypeDefaultAndTeams|1|Dá suporte a ambos `Skype` e `Teams`. O padrão é `Skype`.|
|teamsDefaultAndSkype|2|Dá suporte a ambos `Skype` e `Teams`. O padrão é `Teams`.|
|skypeOnly|3|Dá suporte apenas `Skype`a .|
|teamsOnly|4|Dá suporte apenas `Teams`a .|
|unknownFutureValue|5|Valor de sentinel de enumeração evolvável. Não usar.|

### <a name="longrunningoperationstatus-values"></a>Valores longRunningOperationStatus

| Member|
|:-----------------|
|Notstarted|
|Executando|
|Conseguiu|
|Falhou|
|unknownFutureValue|

### <a name="delegatedadminaccessassignmentstatus-values"></a>Valores delegatedAdminAccessAssignmentStatus 

|Member|
|:---|
|Pendente|
|Ativo|
|Excluir|
|deleted|
|erro|
|unknownFutureValue|

### <a name="delegatedadminaccesscontainertype-values"></a>Valores delegatedAdminAccessContainerType 

|Member|
|:---|
|Securitygroup|
|unknownFutureValue|

### <a name="delegatedadminrelationshipoperationtype-values"></a>Valores delegatedAdminRelationshipOperationType 

|Member|
|:---|
|delegatedAdminAccessAssignmentUpdate|
|unknownFutureValue|

### <a name="delegatedadminrelationshiprequestaction-values"></a>Valores delegatedAdminRelationshipRequestAction 

|Member|
|:---|
|lockForApproval|
|Terminar|
|unknownFutureValue|

### <a name="delegatedadminrelationshiprequeststatus-values"></a>valores delegatedAdminRelationshipRequestStatus 

|Member|
|:---|
|criadas|
|Pendente|
|Conseguiu|
|Falhou|
|unknownFutureValue|

### <a name="delegatedadminrelationshipstatus-values"></a>valores delegatedAdminRelationshipStatus 

|Member|
|:---|
|Ativar|
|Ativo|
|approvalPending|
|Aprovado|
|criadas|
|Expirado|
|Expirando|
|Terminada|
|Terminação|
|terminationRequested|
|unknownFutureValue|
