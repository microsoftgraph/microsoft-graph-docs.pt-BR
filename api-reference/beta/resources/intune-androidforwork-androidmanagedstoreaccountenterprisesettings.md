---
title: tipo de recurso de androidManagedStoreAccountEnterpriseSettings
description: Configurações da empresa para um Android gerenciados repositório de conta.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a14f0327c4a4c4cf2bc78e56b63686208e97d4b1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933810"
---
# <a name="androidmanagedstoreaccountenterprisesettings-resource-type"></a>tipo de recurso de androidManagedStoreAccountEnterpriseSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configurações da empresa para um Android gerenciados repositório de conta.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-get.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|Leia as propriedades e os relacionamentos do objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .|
|[Atualizar androidManagedStoreAccountEnterpriseSettings](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-update.md)|[androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)|Atualize as propriedades de um objeto [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) .|
|[Ação requestSignupUrl](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl.md)|Cadeia de caracteres|Ainda não documentado|
|[Ação completeSignup](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup.md)|Nenhum|Ainda não documentado|
|[Ação syncApps](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps.md)|Nenhum|Ainda não documentado|
|[Ação de desvincular](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind.md)|Nenhum|Ainda não documentado|
|[ação de createGooglePlayWebToken](../api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken.md)|String|Gera um token de web que é usado em um componente incorporável.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O Android armazenar identificador de configurações da empresa de conta|
|bindStatus|[androidManagedStoreAccountBindStatus](../resources/intune-androidforwork-androidmanagedstoreaccountbindstatus.md)|Associe o status do inquilino com a API do EMM Google. Os valores possíveis são: `notBound`, `bound`, `boundAndValidated`, `unbinding`.|
|lastAppSyncDateTime|DateTimeOffset|Hora da conclusão da última sincronização do aplicativo|
|lastAppSyncStatus|[androidManagedStoreAccountAppSyncStatus](../resources/intune-androidforwork-androidmanagedstoreaccountappsyncstatus.md)|Resultado da última sincronização de aplicativo. Os possíveis valores são: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.|
|ownerUserPrincipalName|String|UPN proprietária que criou a empresa|
|ownerOrganizationName|String|Nome da organização usado quando a inclusão Android Enterprise|
|lastModifiedDateTime|DateTimeOffset|Hora da última modificação para configurações da empresa Android|
|enrollmentTarget|[androidManagedStoreAccountEnrollmentTarget](../resources/intune-androidforwork-androidmanagedstoreaccountenrollmenttarget.md)|Indica quais usuários podem inscrever dispositivos no gerenciamento de dispositivos Android Enterprise. Os valores possíveis são: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.|
|targetGroupIds|String collection|Especifica a quais grupos AAD podem registrar dispositivos no gerenciamento de dispositivos do Android for Work se enrollmentTarget estiver definido como 'Direcionado'|
|deviceOwnerManagementEnabled|Booliano|Indica se essa conta é flighting para o gerenciamento de proprietário de dispositivo Android com CloudDPC.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAccountEnterpriseSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
  "id": "String (identifier)",
  "bindStatus": "String",
  "lastAppSyncDateTime": "String (timestamp)",
  "lastAppSyncStatus": "String",
  "ownerUserPrincipalName": "String",
  "ownerOrganizationName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "enrollmentTarget": "String",
  "targetGroupIds": [
    "String"
  ],
  "deviceOwnerManagementEnabled": true
}
```





