---
title: Valores de enumeração
description: Valores de enumeração do Microsoft Graph
ms.openlocfilehash: 2f8bd0065136077cda2228cbec1c2d34d546c7d1
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936322"
---
### <a name="contactrelationship-values"></a>valores de contactRelationship

|Membro|Valor|Descrição|
|:---|:---|:---|
|primário|,0|O pai do usuário.|
|relativo|1| O relativo do usuário.|
|facilita|duas| O auxílio do usuário.|
|Doutor|3D| O médico do usuário.|
|responsável|quatro| O guardião do usuário.|
|pensão|0,5| O filho do usuário.|
|outro|6| Uma relação não especificada com o usuário.|
|unknownFutureValue|178| Valor de marcador para compatibilidade futura.|

### <a name="timezonestandard-values"></a>valores de timeZoneStandard

| Valor
|:-----------------
| Windows
| IANA


### <a name="freebusystatus-values"></a>valores de freeBusyStatus

| Membro            |Valor
|:------------------|:-------
| macro              | ,0
| provisória         | 1
| Atualmente              | duas
| temporária               | 3D
| workingElsewhere  | quatro
| desconhecido           | -1


### <a name="physicaladdresstype-values"></a>valores de physicalAddressType

| Valor
|:-------------------------
| desconhecido 
| Casa
| Business 
| outro


### <a name="attendeetype-values"></a>valores de attendetype

| Valor
|:-------------------------
| obrigatório
| opcional
| recurso


### <a name="externalaudiencescope-values"></a>valores de externalAudienceScope

| Valor
|:-------------------------
| nenhuma
| contactsOnly
| todos os


### <a name="automaticrepliesstatus-values"></a>valores de automaticRepliesStatus

| Valor
|:-------------------------
| deficiência
| alwaysEnabled
| agendado


### <a name="calendarcolor-values"></a>valores de calendarColor

| Membro     | Valor
|:-----------|:----------
| Automático       | -1
| lightBlue  | ,0
| lightGreen | 1
| lightOrange| duas
| lightGray  | 3D
| lightYellow| quatro
| lightTeal  | 0,5
| lightPink  | 6
| lightBrown | 178
| lightRed   | 8
| maxColor   | 241


### <a name="educationsynchronizationprofilestate-values"></a>valores de educationSynchronizationProfileState

| Membro     | Valor
|:-----------|:----------
| deleta          | duas
| deletionFailed    | 3D
| provisioningFailed | 0,5
| provisionado        | 6
| provisionamento       | 178
| unknownFutureValue | 8


### <a name="educationsynchronizationstatus-values"></a>valores de educationSynchronizationStatus

| Membro     | Valor
|:-----------|:----------
| pausado          | ,0
| inProgress    | 1
| sucesso | duas
| erro        | 3D
| validationError | quatro
| em quarentena       | 0,5
| unknownFutureValue | 6

### <a name="educationexternalsource-values"></a>valores de educationExternalSource

| Valor
|:-------------------------
| activa
| Manual
| unknownFutureValue


### <a name="educationgender-values"></a>valores de educationGender

| Valor
|:-------------------------
| feminino
| canto
| outro
| unknownFutureValue


### <a name="eventtype-values"></a>valores de eventType

| Valor
|:-------------------------
| singleInstance
| ocorrência
| exceções
| série


### <a name="sensitivity-values"></a>valores de sensibilidade

| Valor
|:-------------------------
| SS
| pessoal
| privada
| acordo


### <a name="importance-values"></a>valores de importância

| Valor
|:-------------------------
| low
| SS
| high


### <a name="educationuserrole-values"></a>valores de educationUserRole
| Valor
|:---------------------
| student
| teacher
| nenhuma
| unknownFutureValue


### <a name="meetingmessagetype-values"></a>valores de meetingMessageType

| Valor
|:-----------------
| nenhuma
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>valores de followupFlagStatus

| Valor
|:-------------------------
| não sinalizado
| complete
| indicado


### <a name="inferenceclassificationtype-values"></a>valores de inferenceClassificationType

| Valor
|:-----------------
| Destaques
| outro


### <a name="iosnotificationalerttype-values"></a>valores de iosNotificationAlertType

| Valor
|:-------------------------
| deviceDefault
| Bandeira
| JanelaRestrita
| nenhuma

### <a name="deviceenrollmentfailurereason-values"></a>valores de deviceEnrollmentFailureReason

| Valor
|:-------------
| desconhecido
| autentica
| nesse
| accountValidation
| userValidation
| deviceNotSupported
| inManutenção
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### <a name="bodytype-values"></a>valores de BodyType
| Valor
|:---------
| texto
| HTML


### <a name="locationtype-values"></a>valores LocationType

| Valor
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

| Valor
|:-------------------------
| desconhecido
| locationStore
| Directory
| privada
| Bing


### <a name="messageactionflag-values"></a>valores de messageActionFlag

| Valor
|:-------------------------
| qualquer
| call
| doNotForward
| Acompanhamento
| conhecimento
| direta
| noResponseNecessary
| Saiba
| resposta
| replyToAll
| exame


### <a name="onenoteuserrole-values"></a>valores de onenoteUserRole

| Membro      | Valor
|:------------|:------------
| Owner       | ,0
| Colaborador | 1
| Leitor      | duas
| Nenhum        | -1


### <a name="operationstatus-values"></a>valores de operationStatus

| Valor
|:-----------------
| NotStarted
| Executando
| Completed
| Failed


### <a name="onenotepatchactiontype-values"></a>valores de onenotePatchActionType

| Valor
|:-------------------------
| Substituir
| Append
| Excluir
| Insert
| Preceder

### <a name="onenotepatchinsertposition-values"></a>valores de onenotePatchInsertPosition

| Valor
|:-------------------------
| After
| Before


### <a name="phonetype-values"></a>valores de PhoneType

| Valor
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

| Valor
|:-------------------------
| Automático
| noPreview
| verificação
| descrição
| de referência


### <a name="status-values"></a>valores de status

| Valor
|:-----------------
| active
| atualizado
| deleted
| ignor
| unknownFutureValue


### <a name="weekindex-values"></a>valores de weekIndex

| Valor
|:-------------------------
| primeiro
| secundária
| terceiriza
| etapa
| durar


### <a name="dayofweek-values"></a>valores de dayOfWeek

| Valor
|:-------------------------
| domingo
| período
| feira
| feira
| quinta-feira
| sexta
| sábado

### <a name="recurrencepatterntype-values"></a>valores recurrencePattern

| Valor
|:-------------------------
| diariamente
| mensal
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>valores de recurrenceRangeType

| Valor
|:-------------------------
| endDate
| noEnd
| numerada


### <a name="onenotesourceservice-values"></a>valores de onenoteSourceService
| Valor
|:---------------------
| Desconhecido
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>valores ResponseType

| Valor
|:-------------------------
| nenhuma
| organizer
| tentativelyAccepted
| aceito
| recusada
| Não respondido


### <a name="activitydomain-values"></a>valores de activityDomain

| Valor
|:-------------------------
| desconhecido
| trabalho
| pessoal
| irrestrito


### <a name="websitetype-values"></a>valores de WebSiteType

| Valor
|:-------------------------
| outro
| Casa
| trabalho
| blog
| profile


### <a name="categorycolor-values"></a>valores de categoryColor

| Membro   |Valor    
|:---------|:--------
| nenhuma     | -1      
| preset0  | ,0       
| preset1  | 1       
| preset2  | duas       
| preset3  | 3D       
| preset4  | quatro       
| preset5  | 0,5       
| preset6  | 6       
| preset7  | 178       
| preset8  | 8       
| preset9  | 241       
| preset10 | 254      
| preset11 | 11      
| preset12 | 3,6      
| preset13 | Treze      
| preset14 | 14      
| preset15 | 15      
| preset16 | dezesseis      
| preset17 | 17.07.06      
| preset18 | anos      
| preset19 | 19      
| preset20 | 508      
| preset21 | 21      
| preset22 | 22      
| preset23 | 23      
| preset24 | dia      

### <a name="alertfeedback-values"></a>valores de alertFeedback

Possíveis valores de comentários no alerta fornecido por um analista.

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Unknown.|
|truePositive|1|O alerta é verdadeiro e positivo.|
|falsePositive|duas| O alerta é falso positivo.|
|benignPositive|3D| O alerta é benigno-positivo.|

### <a name="filehashtype-values"></a>valores de fileHashtype

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Tipo desconhecido.|
|SHA1|1|Tipo de hash SHA1.|
|SHA256|duas| Tipo de hash SHA256.|
|MD5|3D| Tipo de hash MD5.|
|authenticodeHash256|quatro| Tipo de hash AuthenticodeHash256.|
|lsHash|0,5| Tipo de hash LsHash.|
|ctph|6| Tipo de hash CTPH.|
|peSha1|178| Tipo de hash PESHA1.|
|peSha256|8| Tipo de hash PESHA256.|

### <a name="connectiondirection-values"></a>valores de connectionDirection

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Conexão desconhecida.|
|entrada|1|Conexão de entrada.|
|saída|duas| Conexão de saída.|

### <a name="connectionstatus-values"></a>valores de connectionStatus

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Status de conexão desconhecido.|
|tentou|1|Tentativa de conexão.|
|adicionada|duas| Conexão bem-sucedida.|
|bloqueou|3D| Conexão bloqueada.|
|falhou|quatro| Falha de conexão.|

### <a name="processintegritylevel-values"></a>valores de processIntegrityLevel

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Unknown.|
|não confiáveis|254|O nível de integridade é não confiável.|
|low|508| O nível de integridade é baixo.|
|medium|até| O nível de integridade é médio.|
|high|40| O nível de integridade é alto.|
|sistema|50| O nível de integridade é System.|

### <a name="registryhive-values"></a>valores de registryHive

Enumeração para hives do registro, conforme [https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)definido por.

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Hive desconhecido.|
|currentConfig|1|Hive HKEY_CURRENT_CONFIG.|
|currentUser|duas| Hive HKEY_CURRENT_USER.|
|localMachineSam|3D| Hive HKEY_LOCAL_MACHINE\SAM.|
|localMachineSamSoftware|quatro| Hive HKEY_LOCAL_MACHINE\Software.|
|localMachineSystem|0,5| HKEY_LOCAL_MACHINE\System Hive.|
|usersDefault|6| HKEY_USERS\\. Hive padrão.|

### <a name="registryoperation-values"></a>valores de registryOperation

Operação que alterou o nome da chave do registro e/ou o valor.

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Tipo de valor de registro desconhecido.|
|create|1|Criar registro.|
|modifica|duas|Modificar o registro.|
|delete|3D|Excluir registro.|

### <a name="registryvaluetype-values"></a>valores de registryValueType

Enumeração para tipos de valor do registro conforme [https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types)definido por.

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Tipo de valor de registro desconhecido.|
|binário|1|Tipo de valor de registro REG_BINARY.|
|últimas|duas| Tipo de valor do registro REG_DWORD.|
|dwordLittleEndian|3D| Tipo de valor do registro REG_DWORD_LITTLE_ENDIAN.|
|dwordBigEndian|quatro| Tipo de valor do registro REG_DWORD_BIG_ENDIAN.|
|expandSz|0,5| Tipo de valor do registro REG_EXPAND_SZ.|
|vínculo|6| Tipo de valor do registro REG_LINK.|
|multiSz|178| Tipo de valor de registro REG_MULTI_SZ.|
|nenhuma|8| Tipo de valor do registro REG_NONE.|
|QWORD|241| Tipo de valor do registro REG_QWORD.|
|qwordlittleEndian|254| Tipo de valor do registro REG_QWORD_LITTLE_ENDIAN.|
|v|11| Tipo de valor do registro REG_SZ.|

### <a name="alertseverity-values"></a>valores de alertSeverity

Enumeração para gravidade de alertas.

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|A severidade é desconhecida.|
|informativa|1|A severidade só é para informações.|
|low|duas| A severidade é baixa.|
|medium|3D| A severidade é média.|
|high|quatro| A severidade é alta.|

### <a name="alertstatus-values"></a>valores de alertStatus

Valores possíveis de um status de ciclo de vida de alerta (estágio).

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Status desconhecido.|
|newAlert|254| O alerta é novo.|
|inProgress|508|O alerta está em andamento.|
|Obtido|até|O alerta foi resolvido.|

### <a name="emailrole-values"></a>valores de emailRole

Valores possíveis para funções de email.

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Função desconhecida.|
|remetente|1|Remetente do email.|
|destinatário|duas|Destinatário do email.|

### <a name="logontype-values"></a>valores de Logontype

Valores possíveis para o método de User Sign.

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|-1|Unknown.|
|interativa|,0|O logon é interativo.|
|remoteInteractive|1| O logon é interativo remoto.|
|rede|duas| O logon é rede.|
|batch|3D| O logon é em lote.|
|service|quatro| O logon é serviço.|

### <a name="useraccountsecuritytype-values"></a>valores de userAccountSecurityType

Valores possíveis para tipos de contas de usuário (Associação de grupo), por definição do Windows.

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|-1|Unknown.|
|caracteres|,0|Membro do grupo de usuários padrão.|
|força|1| Membro do grupo de usuários avançados.|
|administrador|duas| Membro do grupo Administradores.|
