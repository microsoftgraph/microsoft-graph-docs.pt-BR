---
title: tipo de recurso de depOnboardingSetting
description: O depOnboardingSetting representa uma instância do serviço Apple DEP sendo onboarded para Intune. A instância do serviço onboarded gerencia um Token Apple usado para sincronizar dados entre Apple e Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e4b45c4a14258fbe53e8cdfd8c5e83b8c858966b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970679"
---
# <a name="deponboardingsetting-resource-type"></a>tipo de recurso de depOnboardingSetting

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O depOnboardingSetting representa uma instância do serviço Apple DEP sendo onboarded para Intune. A instância do serviço onboarded gerencia um Token Apple usado para sincronizar dados entre Apple e Intune.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|coleção [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Lista as propriedades e os relacionamentos dos objetos [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Obter depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Leia as propriedades e os relacionamentos do objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Criar depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Crie um novo objeto de [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Excluir depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-delete.md)|Nenhum|Exclui um [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).|
|[Atualizar depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Atualize as propriedades de um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[função getEncryptionPublicKey](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|Cadeia de caracteres|Obtenha uma chave pública para usar para criptografar o programa de inscrição do dispositivo Apple token|
|[ação de uploadDepToken](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|Nenhum|Carrega um novo token do programa de inscrição do dispositivo|
|[ação de syncWithAppleDeviceEnrollmentProgram](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|Nenhum|Sincroniza entre Intune e o programa de inscrição do dispositivo Apple|
|[ação de shareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|Nenhum|Ainda não documentado|
|[ação de unshareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O UUID do objeto.|
|appleIdentifier|Cadeia de caracteres|A ID do Apple usada para obter o token atual.|
|tokenExpirationDateTime|DateTimeOffset|Quando o token irá expirar.|
|lastModifiedDateTime|DateTimeOffset|Quando o serviço foi onboarded.|
|lastSuccessfulSyncDateTime|DateTimeOffset|Quando o syned última do serviço com Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Quando o Intune solicitado último uma sincronização.|
|shareTokenWithSchoolDataSyncService|Booliano|Ou não o compartilhamento token do Dep está habilitado com o serviço de sincronização de dados da escola.|
|lastSyncErrorCode|Int32|Código de erro relatado pelo Apple durante a última sincronização dep.|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|Obtém ou define o tipo de Token do Dep. Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.|
|tokenName|Cadeia de caracteres|Nome amigável para o Token de Dep|
|syncedDeviceCount|Int32|Obtém sincronizados contagem de dispositivo|
|defaultProfileDisplayName|Cadeia de caracteres|Obtém sincronizados contagem de dispositivo|
|dataSharingConsentGranted|Booliano|Concedido consentimento para o compartilhamento de dados com Apple Dep Service|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|IOS padrão perfil de inscrição|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Perfil de inscrição MacOs padrão|
|enrollmentProfiles|coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Os perfis de inscrição.|
|importedAppleDeviceIdentities|coleção [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|As identidades de dispositivo Apple importadas.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depOnboardingSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depOnboardingSetting",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "tokenExpirationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastSuccessfulSyncDateTime": "String (timestamp)",
  "lastSyncTriggeredDateTime": "String (timestamp)",
  "shareTokenWithSchoolDataSyncService": true,
  "lastSyncErrorCode": 1024,
  "tokenType": "String",
  "tokenName": "String",
  "syncedDeviceCount": 1024,
  "defaultProfileDisplayName": "String",
  "dataSharingConsentGranted": true
}
```





