---
title: Criar groupPolicyMigrationReport
description: Crie um novo objeto groupPolicyMigrationReport.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5306fe772bc36c9de10a74227ce04f626ce82b81
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59065208"
---
# <a name="create-grouppolicymigrationreport"></a>Criar groupPolicyMigrationReport

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto groupPolicyMigrationReport.

A tabela a seguir mostra as propriedades que são necessárias ao criar o groupPolicyMigrationReport.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Ainda não documentado|
|groupPolicyObjectId|Guid|O GUID do objeto de política de grupo do conteúdo XML do GPO|
|displayName|Cadeia de caracteres|O nome do Objeto de Política de Grupo do Conteúdo XML do GPO|
|ouDistinguishedName|Cadeia de Caracteres|O nome diferenciado da UO.|
|createdDateTime|DateTimeOffset|A data e a hora em que o GroupPolicyMigrationReport foi criado.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que GroupPolicyMigrationReport foi modificada pela última vez.|
|groupPolicyCreatedDateTime|DateTimeOffset|A data e a hora em que o GroupPolicyMigrationReport foi criado.|
|groupPolicyLastModifiedDateTime|DateTimeOffset|A data e a hora em que GroupPolicyMigrationReport foi modificada pela última vez.|
|migrationReadiness|[groupPolicyMigrationReadiness](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|A cobertura do Intune para o arquivo de Objeto de Política de Grupo associado. Os valores possíveis são: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|targetedInActiveDirectory|Boleano|A propriedade Targeted in AD do Conteúdo XML do GPO|
|totalSettingsCount|Int32|O número total de políticas de grupo Configurações do arquivo GPO.|
|supportedSettingsCount|Int32|O número de políticas de grupo Configurações com suporte do Intune.|
|supportedSettingsPercent|Int32|O Percentual de políticas de grupo Configurações com suporte do Intune.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 716

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```



