---
title: Valores de enumeração
description: Valores de enumeração do Microsoft Graph
doc_type: enumPageType
localization_priority: Normal
ms.prod: non-product-specific
author: MSGraphDocsvTeam
ms.openlocfilehash: 67b55dc01cbbc9ae5188e93a5bf24248e2ded483
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948384"
---
# <a name="enum-values"></a>Valores de enumeração

Namespace: microsoft.graph

### <a name="attachmenttype-values"></a>valores AttachmentType

| Member
|:--------------
| file
| item
| de referência

### <a name="analyticsactivitytype-values"></a>valores de analyticsActivityType

| Member
|:--------------
| call
| chat
| email
| foco
| Atenda

### <a name="registrationauthmethod-values"></a>valores de registrationAuthMethod

|Member|
|:---|
|email|
|mobilePhone|
|officePhone|
|securityQuestion|
|appNotification|
|appCode|
|alternateMobilePhone|

### <a name="entitytypes-values"></a>valores de entityTypes

|Member|
|:---|
|Microsoft. Graph. Event|
|Microsoft. Graph. Message|
|Microsoft. Graph. driveItem|
|Microsoft. Graph. externalfile|
|Microsoft. Graph. externalItem|

### <a name="contactrelationship-values"></a>valores de contactRelationship

| Membro             | Valor | Descrição                              |
| :----------------- | :---- | :--------------------------------------- |
| primário             | ,0     | O pai do usuário.                       |
| relativo           | 1     | O relativo do usuário.                     |
| facilita               | duas     | O auxílio do usuário.                         |
| Doutor             | 3D     | O médico do usuário.                       |
| responsável           | 4      | O guardião do usuário.                     |
| pensão              | 5      | O filho do usuário.                        |
| outro              | 6      | Uma relação não especificada com o usuário. |
| unknownFutureValue | 7      | Valor de marcador para compatibilidade futura.   |

### <a name="scheduleentitytheme-values"></a>valores de scheduleEntityTheme

| Member
|:-------------------------
| branco
| azuis
| natureza
| roxa
| Rosa
| amarelo
| acinzentada
| darkBlue
| darkGreen
| darkPurple
| darkPink
| darkYellow
| unknownFutureValue


### <a name="timeoffreasonicontype-values"></a>valores de timeOffReasonIconType

|Member|
|:---|
|nenhuma|
|automóvel|
|calendar|
|com|
|plano|
|firstAid|
|Doutor|
|Não trabalho|
|medição|
|juryDuty|
|Globe|
|copo|
|phone|
|clima|
|abrangência|
|piggyBank|
|cachorro|
|torta|
|trafficCone|
|pessoal|
|ensolarado|
|unknownFutureValue|

### <a name="schedulechangestate-values"></a>valores de scheduleChangeState

| Member
|:----------------------------
|função
|pelos
|recusada
|unknownFutureValue

### <a name="schedulechangerequestactor-values"></a>valores de scheduleChangeRequestActor

| Member
|:----------------------------
|remetente
|destinatário
|manager
|sistema
|unknownFutureValue

### <a name="workforceintegrationencryptionprotocol-values"></a>valores de workforceIntegrationEncryptionProtocol

| Member
|:----------------------------
|sharedSecret
|unknownFutureValue

### <a name="workforceintegrationsupportedentities-values"></a>valores de workforceIntegrationSupportedEntities

| Member
|:----------------------------
|nenhuma
|shift
|swapRequest
|openShift
|openShiftRequest
|userShiftPreferences

### <a name="timezonestandard-values"></a>valores de timeZoneStandard

| Member
|:-----------------
| Windows
| IANA


### <a name="freebusystatus-values"></a>valores de freeBusyStatus

| Membro           | Valor |
| :--------------- | :---- |
| macro             | ,0     |
| provisória        | 1     |
| Atualmente             | duas     |
| temporária              | 3D     |
| workingElsewhere | 4      |
| desconhecido          | -1    |


### <a name="physicaladdresstype-values"></a>valores de physicalAddressType

| Member
|:-------------------------
| desconhecido
| Casa
| Business
| outro


### <a name="attendeetype-values"></a>valores de attendetype

| Member
|:-------------------------
| obrigatório
| opcional
| recurso


### <a name="externalaudiencescope-values"></a>valores de externalAudienceScope

| Member
|:-------------------------
| nenhuma
| contactsOnly
| todos os


### <a name="automaticrepliesstatus-values"></a>valores de automaticRepliesStatus

| Member
|:-------------------------
| deficiência
| alwaysEnabled
| agendado


### <a name="calendarcolor-values"></a>valores de calendarColor

| Membro      | Valor |
| :---------- | :---- |
| Automático        | -1    |
| lightBlue   | ,0     |
| lightGreen  | 1     |
| lightOrange | duas     |
| lightGray   | 3D     |
| lightYellow | 4      |
| lightTeal   | 5      |
| lightPink   | 6      |
| lightBrown  | 7      |
| lightRed    | 8      |
| maxColor    | 9      |


### <a name="educationsynchronizationprofilestate-values"></a>valores de educationSynchronizationProfileState

| Membro             | Valor |
| :----------------- | :---- |
| deleta           | duas     |
| deletionFailed     | 3D     |
| provisioningFailed | 5      |
| provisionado        | 6      |
| provisionamento       | 7      |
| unknownFutureValue | 8      |


### <a name="educationsynchronizationstatus-values"></a>valores de educationSynchronizationStatus

| Membro             | Valor |
| :----------------- | :---- |
| pausado             | ,0     |
| inProgress         | 1     |
| sucesso            | duas     |
| erro              | 3D     |
| validationError    | 4      |
| em quarentena        | 5      |
| unknownFutureValue | 6      |

### <a name="educationexternalsource-values"></a>valores de educationExternalSource

| Member
|:-------------------------
| activa
| Manual
| unknownFutureValue


### <a name="educationgender-values"></a>valores de educationGender

| Member
|:-------------------------
| feminino
| canto
| outro
| unknownFutureValue


### <a name="eventtype-values"></a>valores de eventType

| Member
|:-------------------------
| singleInstance
| ocorrência
| exceções
| série


### <a name="sensitivity-values"></a>valores de sensibilidade

| Member
|:-------------------------
| SS
| pessoal
| privada
| acordo


### <a name="importance-values"></a>valores de importância

| Member
|:-------------------------
| low
| SS
| high


### <a name="educationuserrole-values"></a>valores de educationUserRole
| Member
|:---------------------
| student
| teacher
| docentes


### <a name="meetingmessagetype-values"></a>valores de meetingMessageType

| Member
|:-----------------
| nenhuma
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>valores de followupFlagStatus

| Member
|:-------------------------
| não sinalizado
| complete
| indicado


### <a name="inferenceclassificationtype-values"></a>valores de inferenceClassificationType

| Member
|:-----------------
| Destaques
| outro


### <a name="iosnotificationalerttype-values"></a>valores de iosNotificationAlertType

| Member
|:-------------------------
| deviceDefault
| Bandeira
| JanelaRestrita
| nenhuma

### <a name="deviceenrollmentfailurereason-values"></a>valores de deviceEnrollmentFailureReason

| Member
|:-------------
| desconhecido
| autentica
| nesse
| accountValidation
| uservalidation
| deviceNotSupported
| inmanutenção
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### <a name="bodytype-values"></a>valores de BodyType
| Member
|:---------
| texto
| HTML


### <a name="locationtype-values"></a>valores LocationType

| Member
|:-------------------------
| Padrão.
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| diárias
| restaurantes
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>valores de locationUniqueIdType

| Member
|:-------------------------
| desconhecido
| locationStore
| Directory
| privada
| Bing


### <a name="messageactionflag-values"></a>valores de messageActionFlag

| Member
|:-------------------------
| qualquer
| call
| doNotForward
| Acompanhamento
| conhecimento
| forward
| noResponseNecessary
| Saiba
| reply
| replyToAll
| exame


### <a name="onenoteuserrole-values"></a>valores de onenoteUserRole

| Membro      | Valor |
| :---------- | :---- |
| Proprietário       | ,0     |
| Colaborador | 1     |
| Leitor      | duas     |
| Nenhum        | -1    |


### <a name="operationstatus-values"></a>valores de operationStatus

| Member
|:-----------------
| NotStarted
| Em execução
| Completed
| Falhou


### <a name="onenotepatchactiontype-values"></a>valores de onenotePatchActionType

| Member
|:-------------------------
| Substituir
| Append
| Excluir
| Inserir
| Preceder

### <a name="onenotepatchinsertposition-values"></a>valores de onenotePatchInsertPosition

| Member
|:-------------------------
| After
| Before


### <a name="phonetype-values"></a>valores de PhoneType

| Member
|:-------------------------
| Casa
| Business
| processadores
| outro
| assistência
| homeFax
| businessFax
| otherFax
| pager
| Radio


### <a name="plannerpreviewtype-values"></a>valores de plannerPreviewType

| Member
|:-------------------------
| Automático
| nopreview
| verificação
| description
| de referência


### <a name="status-values"></a>valores de status

| Member
|:-----------------
| active
| atualizado
| deleted
| ignor
| unknownFutureValue


### <a name="weekindex-values"></a>valores de weekIndex

| Member
|:-------------------------
| primeiro
| secundária
| terceiriza
| etapa
| durar


### <a name="dayofweek-values"></a>valores de dayOfWeek

| Member
|:-------------------------
| domingo
| período
| feira
| feira
| quinta-feira
| sexta
| sábado

### <a name="recurrencepatterntype-values"></a>valores recurrencePattern

| Member
|:-------------------------
| diariamente
| mensal
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>valores de recurrenceRangeType

| Member
|:-------------------------
| endDate
| noEnd
| numerada


### <a name="onenotesourceservice-values"></a>valores de onenoteSourceService
| Member
|:---------------------
| Desconhecido
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>valores ResponseType

| Member
|:-------------------------
| nenhuma
| organizer
| tentativelyAccepted
| aceito
| recusada
| Não respondido


### <a name="activitydomain-values"></a>valores de activityDomain

| Member
|:-------------------------
| desconhecido
| trabalho
| pessoal
| irrestrito


### <a name="websitetype-values"></a>valores de WebSiteType

| Member
|:-------------------------
| outro
| Casa
| trabalho
| blog
| perfil


### <a name="categorycolor-values"></a>valores de categoryColor

| Membro   | Valor |
| :------- | :---- |
| nenhuma     | -1    |
| preset0  | ,0     |
| preset1  | 1     |
| preset2  | duas     |
| preset3  | 3D     |
| preset4  | 4      |
| preset5  | 5      |
| preset6  | 6      |
| preset7  | 7      |
| preset8  | 8      |
| preset9  | 9      |
| preset10 | 10     |
| preset11 | 11    |
| preset12 | 12     |
| preset13 | 13     |
| preset14 | 14     |
| preset15 | 15     |
| preset16 | 16     |
| preset17 | 17     |
| preset18 | 18     |
| preset19 | 19    |
| preset20 | 508    |
| preset21 | 21    |
| preset22 | 22    |
| preset23 | 23    |
| preset24 | dia    |

### <a name="alertfeedback-values"></a>valores de alertFeedback

Possíveis valores de comentários no alerta fornecido por um analista.

| Membro         | Valor | Descrição               |
| :------------- | :---- | :------------------------ |
| desconhecido        | ,0     | Unknown.                  |
| truePositive   | 1     | O alerta é verdadeiro e positivo.   |
| falsePositive  | duas     | O alerta é falso positivo.  |
| benignPositive | 3D     | O alerta é benigno-positivo. |

### <a name="filehashtype-values"></a>valores de filehashtype

| Membro              | Valor | Descrição                    |
| :------------------ | :---- | :----------------------------- |
| desconhecido             | ,0     | Tipo desconhecido.                  |
| SHA1                | 1     | Tipo de hash SHA1.                |
| SHA256              | duas     | Tipo de hash SHA256.              |
| MD5                 | 3D     | Tipo de hash MD5.                 |
| authenticodeHash256 | 4      | Tipo de hash AuthenticodeHash256. |
| lsHash              | 5      | Tipo de hash LsHash.              |
| ctph                | 6      | Tipo de hash CTPH.                |
| peSha1              | 7      | Tipo de hash PESHA1.              |
| peSha256            | 8      | Tipo de hash PESHA256.            |

### <a name="connectiondirection-values"></a>valores de connectionDirection

| Membro   | Valor | Descrição          |
| :------- | :---- | :------------------- |
| desconhecido  | ,0     | Conexão desconhecida.  |
| entrada  | 1     | Conexão de entrada.  |
| saída | duas     | Conexão de saída. |

### <a name="connectionstatus-values"></a>valores de connectionStatus

| Membro    | Valor | Descrição                |
| :-------- | :---- | :------------------------- |
| desconhecido   | ,0     | Status de conexão desconhecido. |
| tentou | 1     | Tentativa de conexão.      |
| adicionada | duas     | Conexão bem-sucedida.      |
| bloqueou   | 3D     | Conexão bloqueada.        |
| falhou    | 4      | Falha de conexão.         |

### <a name="processintegritylevel-values"></a>valores de processIntegrityLevel

| Membro    | Valor | Descrição                   |
| :-------- | :---- | :---------------------------- |
| desconhecido   | ,0     | Unknown.                      |
| não confiáveis | 10     | O nível de integridade é não confiável. |
| low       | 508    | O nível de integridade é baixo.       |
| medium    | até    | O nível de integridade é médio.    |
| high      | 40    | O nível de integridade é alto.      |
| sistema    | 50    | O nível de integridade é System.    |

### <a name="registryhive-values"></a>valores de registryHive

Enumeração para hives do registro, conforme [https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives](https://docs.microsoft.com/windows/desktop/sysinfo/registry-hives)definido por.

| Membro                  | Valor | Descrição                       |
| :---------------------- | :---- | :-------------------------------- |
| desconhecido                 | ,0     | Hive desconhecido.                     |
| currentConfig           | 1     | HKEY_CURRENT_CONFIG Hive.         |
| currentUser             | duas     | HKEY_CURRENT_USER Hive.           |
| localMachineSam         | 3D     | HKEY_LOCAL_MACHINE Hive \SAM.      |
| localMachineSamSoftware | 4      | HKEY_LOCAL_MACHINE seção \Software. |
| localMachineSystem      | 5      | HKEY_LOCAL_MACHINE o hive de \System.   |
| usersDefault            | 6      | HKEY_USERS\\. Hive padrão.        |

### <a name="registryoperation-values"></a>valores de registryOperation

Operação que alterou o nome da chave do registro e/ou o valor.

| Membro  | Valor | Descrição                  |
| :------ | :---- | :--------------------------- |
| desconhecido | ,0     | Tipo de valor de registro desconhecido. |
| create  | 1     | Criar registro.             |
| modifica  | duas     | Modificar o registro.             |
| delete  | 3D     | Excluir registro.             |

### <a name="registryvaluetype-values"></a>valores de registryValueType

Enumeração para tipos de valor do registro, conforme definido pelos [tipos de valor do registro](https://docs.microsoft.com/windows/desktop/sysinfo/registry-value-types).

| Membro            | Valor | Descrição                                  |
| :---------------- | :---- | :------------------------------------------- |
| desconhecido           | ,0     | Tipo de valor de registro desconhecido.                 |
| binário            | 1     | REG_BINARY tipo de valor do registro.              |
| últimas             | duas     | REG_DWORD tipo de valor do registro.               |
| dwordLittleEndian | 3D     | REG_DWORD_LITTLE_ENDIAN tipo de valor do registro. |
| dwordBigEndian    | 4      | REG_DWORD_BIG_ENDIAN tipo de valor do registro.    |
| expandSz          | 5      | REG_EXPAND_SZ tipo de valor do registro.           |
| vínculo              | 6      | REG_LINK tipo de valor do registro.                |
| multiSz           | 7      | REG_MULTI_SZ tipo de valor do registro.            |
| nenhuma              | 8      | REG_NONE tipo de valor do registro.                |
| QWORD             | 9      | REG_QWORD tipo de valor do registro.               |
| qwordlittleEndian | 10     | REG_QWORD_LITTLE_ENDIAN tipo de valor do registro. |
| v                | 11    | REG_SZ tipo de valor do registro.                  |

### <a name="alertseverity-values"></a>valores de alertSeverity

Enumeração para gravidade de alertas.

| Membro        | Valor | Descrição                       |
| :------------ | :---- | :-------------------------------- |
| desconhecido       | ,0     | A severidade é desconhecida.              |
| informativa | 1     | A severidade só é para informações. |
| low           | duas     | A severidade é baixa.                  |
| medium        | 3D     | A severidade é média.               |
| high          | 4      | A severidade é alta.                 |

### <a name="alertstatus-values"></a>valores de alertStatus

Valores possíveis de um status de ciclo de vida de alerta (estágio).

| Membro     | Valor | Descrição           |
| :--------- | :---- | :-------------------- |
| desconhecido    | ,0     | Status desconhecido.       |
| newAlert   | 10     | O alerta é novo.         |
| inProgress | 508    | O alerta está em andamento. |
| Obtido   | até    | O alerta foi resolvido.    |

### <a name="emailrole-values"></a>valores de emailRole

Valores possíveis para funções de email.

| Membro    | Valor | Descrição             |
| :-------- | :---- | :---------------------- |
| desconhecido   | ,0     | Função desconhecida.           |
| remetente    | 1     | Remetente do email.    |
| destinatário | duas     | Destinatário do email. |

### <a name="logontype-values"></a>valores de Logontype

Valores possíveis para o método de User Sign.

| Membro            | Valor | Descrição                  |
| :---------------- | :---- | :--------------------------- |
| desconhecido           | -1    | Unknown.                     |
| interativa       | ,0     | O logon é interativo.        |
| remoteInteractive | 1     | O logon é interativo remoto. |
| rede           | duas     | O logon é rede.            |
| batch             | 3D     | O logon é em lote.              |
| service           | 4      | O logon é serviço.            |

### <a name="useraccountsecuritytype-values"></a>valores de userAccountSecurityType

Valores possíveis para tipos de contas de usuário (Associação de grupo), por definição do Windows.

| Membro        | Valor | Descrição                     |
| :------------ | :---- | :------------------------------ |
| desconhecido       | -1    | Unknown.                        |
| caracteres      | ,0     | Membro do grupo de usuários padrão. |
| força         | 1     | Membro do grupo de usuários avançados.    |
| administrador | duas     | Membro do grupo Administradores. |

### <a name="scopeoperatormultivaluedcomparisontype-values"></a>valores de scopeOperatorMultiValuedComparisonType

|Member|
|:---|
|todos os|
|qualquer|

### <a name="risklevel-values"></a>valores de riskLevel

|Member|
|:---|
|low|
|medium|
|high|
|hidden|
|nenhuma|
|unknownFutureValue|

### <a name="riskstate-values"></a>valores de risco

|Member|
|:---|
|nenhuma|
|confirmedSafe|
|corrigidos|
|Descartado pelo|
|atRisk|
|confirmedCompromised|
|unknownFutureValue|

### <a name="riskdetail-values"></a>valores de riskDetail

|Member|
|:---|
|nenhuma|
|adminGeneratedTemporaryPassword|
|userPerformedSecuredPasswordChange|
|userPerformedSecuredPasswordReset|
|adminConfirmedSigninSafe|
|aiConfirmedSigninSafe|
|userPassedMFADrivenByRiskBasedPolicy|
|adminDismissedAllRiskForUser|
|adminConfirmedSigninCompromised|
|adminConfirmedUserCompromised|
|hidden|
|unknownFutureValue|

### <a name="referenceattachmentpermission-values"></a>valores de referenceAttachmentPermission

|Member|
|:---|
|outro|
|modo de exibição|
|edit|
|anonymousView|
|anonymousEdit|
|organizationView|
|organizationEdit|

### <a name="referenceattachmentprovider-values"></a>valores de referenceAttachmentProvider

|Member|
|:---|
|outro|
|oneDriveBusiness|
|oneDriveConsumer|
|Dropbox|

### <a name="riskeventtype-values"></a>valores de riskEventType

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
|genérico|
|adminConfirmedUserCompromised|
|mcasImpossibleTravel|
|mcasSuspiciousInboxManipulationRules|
|investigationsThreatIntelligenceSigninLinked|
|maliciousIPAddressValidCredentialsBlockedIP|
|unknownFutureValue|

### <a name="networktype-values"></a>valores de NetworkType

|Member|
|:---|
|Internet|
|extranet|
|namedNetwork|
|confiáveis|
|unknownFutureValue|

### <a name="exchangeidformat-values"></a>valores de exchangeIdFormat

|Member|
|:---|
|entryId|
|ewsId|
|immutableEntryId|
|restid|
|restImmutableEntryId|

### <a name="attributeflowbehavior-values"></a>valores de attributeFlowBehavior

|Member|
|:---|
|flowWhenChanged|
|flowAlways|

### <a name="attributeflowtype-values"></a>valores de attributeFlowType

|Member|
|:---|
|permanente|
|objectaddonamente|
|multiValueAddOnly|
|restid|

### <a name="objectflowtypes-values"></a>valores de objectFlowTypes

| Membro | Valor |
| :----- | :---- |
| Nenhuma   | ,0     |
| Adicionar    | 1     |
| Atualizar | duas     |
| Delete | 4      |

### <a name="chatmessagetype-values"></a>valores de chatMessageType

|Member|
|:---|
|message|

### <a name="chatmessageimportance-values"></a>valores de chatMessageImportance

|Member|
|:---|
|SS|
|high|
|urgente|

### <a name="channelmembershiptype-values"></a>valores de channelMembershipType

| Membro             | Valor |
| :----------------- | :---- |
| caracteres           | ,0     |
| privada            | 1     |
| unknownFutureValue | duas     |

### <a name="stagedfeaturename-values"></a>valores de stagedFeatureName

| Member                    | Descrição                   |
| :------------------------ | :---------------------------- |
| passthroughAuthentication | Autenticação de passagem    |
| seamlessSso               | Logon único contínuo       |
| passwordHashSync          | Sincronização de hash de senha |

### <a name="tokenissuertype-values"></a>valores de tokenIssuerType

|Member|
|:---|
|AzureAD|
|ADFederationServices|
|unknownFutureValue|

### <a name="riskdetectiontimingtype-values"></a>valores de riskDetectionTimingType

|Member|
|:---|
|Não definido|
|Realtime|
|nearRealtime|
|modo|
|unknownFutureValue|

### <a name="activitytype-values"></a>valores de ActivityType

|Member|
|:---|
|SignIn|
|user|
|unknownFutureValue|

### <a name="entitytype-values"></a>valores de entityType

| Member       |
|:--------------|
|event|
|message|
|driveItem|
|externalFile|
|externalItem|

### <a name="onlinemeetingprovidertype-values"></a>valores de onlineMeetingProviderType

|Member|
|:---|
|desconhecido|
|skypeForBusiness|
|skypeForConsumer|
|teamsForBusiness|

### <a name="delegatemeetingmessagedeliveryoptions-values"></a>valores de delegateMeetingMessageDeliveryOptions

|Member|
|:---|
|sendToDelegateAndInformationToPrincipal|
|sendToDelegateAndPrincipal|
|sendToDelegateOnly|

### <a name="calendarroletype-values"></a>valores de calendarRoleType

|Member|
|:---|
|nenhuma|
|freeBusyRead|
|limitedRead|
|Saiba|
|gravável|
|delegateWithoutPrivateEventAccess|
|delegateWithPrivateEventAccess|
|cliente|

### <a name="contentformat-values"></a>valores de contentFormat

| Membro  | Valor | Descrição                          |
| :------ | :---- | :----------------------------------- |
| Padrão. | ,0     | O conteúdo é um tipo de arquivo ou não de email. |
| email   | 1     | O conteúdo é um email.                 |

### <a name="contentstate-values"></a>valores de contentstate

| Membro | Valor | Descrição                                                                      |
| :----- | :---- | :------------------------------------------------------------------------------- |
| descanso   | ,0     | Os dados estão em repouso; Um arquivo em um compartilhamento, por exemplo.                                 |
| movimento | 1     | Os dados estão em movimento. Um arquivo interceptado por um dispositivo de rede em trânsito.         |
| Use    | duas     | Os dados estão em uso. Um arquivo é aberto em um aplicativo cliente como o Microsoft Office. |

### <a name="assignmentmethod-values"></a>valores de AssignmentMethod for utilizado

| Membro     | Valor | Descrição                                                                                                                      |
| :--------- | :---- | :------------------------------------------------------------------------------------------------------------------------------- |
| caracteres   | ,0     | O rótulo foi definido por uma condição de serviço ou política.                                                                              |
| Privilege | 1     | O rótulo foi definido explicitamente por um usuário.                                                                                          |
| Automático       | duas     | Permite a substituição de qualquer rótulo existente. Justificativa necessária no downgrade. Resulta em `standard` método de atribuição em metadados. |

### <a name="actionsource-values"></a>valores de ActionName

| Membro        | Valor | Descrição                                                  |
| :------------ | :---- | :----------------------------------------------------------- |
| Manual        | ,0     | Um usuário selecionou manualmente o rótulo.                          |
| Automático     | 1     | O rótulo foi escolhido como resultado de condições da política.       |
| recomendado   | duas     | O optou por aplicar um rótulo recomendado.                    |
| policyDefault | 3D     | O usuário não ação e o rótulo de política padrão foi aplicado. |
| alguma     | 4      | O usuário escolheu um rótulo depois de ser forçado a escolher.         |

### <a name="contentalignment-values"></a>valores de contentAlignment

| Membro | Valor | Descrição                         |
| :----- | :---- | :---------------------------------- |
| left   | ,0     | Alinha a marcação de conteúdo à esquerda.  |
| Certo  | 1     | Alinha a marcação de conteúdo à direita. |
| Centro | duas     | Centralizar a marcação de conteúdo.             |

### <a name="watermarklayout-values"></a>valores de watermarkLayout

| Membro     | Valor | Descrição                 |
| :--------- | :---- | :-------------------------- |
| horizontal | ,0     | Use uma marca d' água horizontal. |
| diagonal   | 1     | Use uma marca d' água diagonal.   |

### <a name="conditionalaccesspolicystate"></a>conditionalAccessPolicyState

|Member|
|:---|
|enabled|
|deficiência|

### <a name="conditionalaccessclientapp"></a>conditionalAccessClientApp

| Member       |
|:--------------|
|Navegador|
|moderno|
|easSupported|
|easUnsupported|
|outro|

### <a name="conditionalaccessgrantcontrol"></a>conditionalAccessGrantControl

| Member       |
|:--------------|
|Larga|
|fato|
|compliantDevice|
|domainJoinedDevice|
|approvedApplication|
|compliantApplication|

### <a name="cloudappsecuritysessioncontroltype"></a>cloudAppSecuritySessionControlType

| Member       |
|:--------------|
|mcasConfigured|
|monitorOnly|
|blockDownloads|

### <a name="signinfrequencytype"></a>signinFrequencyType

| Member       |
|:--------------|
|durante|
|hora|

### <a name="persistentbrowsersessionmode"></a>persistentBrowserSessionMode

| Member       |
|:--------------|
|permanente|
|Édito|

### <a name="conditionalaccessdeviceplatform"></a>conditionalAccessDevicePlatform

| Member       |
|:--------------|
|Android|
|iOS|
|Windows|
|Windowsphonee|
|macOS|
|todos os|

### <a name="priority-values"></a>valores de prioridade

|Membro|Valor|
|:---|:---|
|Nenhuma|,0|
|Alta|1|
|Baixo|duas|

### <a name="threatassessmentcontenttype-values"></a>valores de threatAssessmentContentType

| Membro | Valor | Descrição             |
|:-------|:------|:------------------------|
| Email   | 1     | Ameaça de email.            |
| url    | duas     | Ameaça de URL.             |
| file   | 3D     | Ameaça do arquivo de anexo. |

### <a name="threatexpectedassessment-values"></a>valores de threatExpectedAssessment

| Membro  | Valor | Descrição                       |
|:--------|:------|:----------------------------------|
| Larga   | 1     | A ameaça deve ser bloqueada.     |
| bloqueia | duas     | A ameaça não deve ser bloqueada. |

### <a name="threatcategory-values"></a>valores de threatCategory

| Membro             | Valor | Descrição        |
|:-------------------|:------|:-------------------|
| electrónico               | 1     | Ameaça de spam.       |
| fraude           | duas     | Ameaça de phishing.   |
| software            | 3D     | Ameaça de malware.    |
| unknownFutureValue | 4      | Um membro Sentinel. |

### <a name="threatassessmentstatus-values"></a>valores de threatAssessmentStatus

| Membro    | Valor | Descrição                              |
|:----------|:------|:-----------------------------------------|
| função   | 1     | A avaliação de ameaças ainda está em andamento. |
| Completed | duas     | A avaliação de ameaças foi concluída.         |

### <a name="threatassessmentrequestsource-values"></a>valores de threatAssessmentRequestSource

| Membro        | Valor | Descrição              |
|:--------------|:------|:-------------------------|
| indefinido     | ,0     | Ainda não conhece.            |
| user          | 1     | Envio do usuário.         |
| administrador | duas     | Envio de administrador de locatários. |

### <a name="threatassessmentresulttype-values"></a>valores de threatAssessmentResultType

| Membro             | Valor | Descrição                                          |
|:-------------------|:------|:-----------------------------------------------------|
| checkPolicy        | 1     | O resultado da verificação de política, `mail` apenas para avaliação. |
| reexaminar             | duas     | O resultado da nova verificação.                                   |
| unknownFutureValue | 3D     | Um membro Sentinel.                                   |

### <a name="maildestinationroutingreason-values"></a>valores de mailDestinationRoutingReason

| Membro                | Valor | Descrição                         |
|:----------------------|:------|:------------------------------------|
| nenhuma                  | ,0     | Ainda não conhece.                       |
| mailFlowRule          | 1     | Regra de transporte do Exchange.            |
| safeSender            | duas     | Lista de remetentes seguros.                   |
| blockedSender         | 3D     | Lista de remetentes bloqueados.                |
| advancedSpamFiltering | 4      | Opção de flitering de spam avançada.     |
| domainAllowList       | 5      | Lista de permissões de domínio do remetente.           |
| domainBlockList       | 6      | Lista de bloqueios de domínio do remetente.           |
| notInAddressBook      | 7      | Excluir o remetente não está no catálogo de endereços. |
| firstTimeSender       | 8      | Bloqueado devido ao remetente pela primeira vez.   |
| autoPurgeToInbox      | 9      | Mensagem de movimentação de viagem para a caixa de entrada.   |
| autoPurgeToJunk       | 10     | Mensagem de movimentação de viagens para lixo eletrônico.    |
| autoPurgeToDeleted    | 11    | Mensagem de movimentação de viagens para exclusão. |
| saída              | 12     | Emails de saída.                      |
| Não é lixo eletrônico               | 13     | Permitir por não ser lixo eletrônico.              |
| desejado                  | 14     | Bloqueado devido a lixo eletrônico.                |
| unknownFutureValue    | 15     | Um membro Sentinel.                  |

### <a name="threatassessmentrequestpivotproperty-values"></a>valores de threatAssessmentRequestPivotProperty

| Membro                       | Valor | Descrição                                                            |
|:-----------------------------|:------|:-----------------------------------------------------------------------|
| threatCategory               | 1     | Agregar solicitação de avaliação `threatCategory`de ameaça por.               |
| mailDestinationRoutingReason | duas     | Agregar solicitação de avaliação `mailDestinationRoutingReason`de ameaça por. |

### <a name="riskeventtypes-values"></a>valores de riskEventTypes

| Member
|:-------------------------
| unlikelyTravel
| anonymizedIPAddress
| maliciousIPAddress
| unfamiliarFeatures
| malwareInfectedIPAddress
| suspiciousIPAddress
| leakedCredentials
| investigationsThreatIntelligence
| genérico
| unknownFutureValue