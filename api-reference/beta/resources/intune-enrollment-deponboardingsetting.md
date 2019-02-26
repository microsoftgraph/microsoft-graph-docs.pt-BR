---
title: tipo de recurso depOnboardingSetting
description: O depOnboardingSetting representa uma instância do serviço Apple DEP que está sendo integrado ao Intune. A instância de serviço integrada gerencia um token Apple usado para sincronizar dados entre o Apple e o Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a3c19a791f97b7cb40bdd2398fec4c1812fdcde
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145280"
---
# <a name="deponboardingsetting-resource-type"></a>tipo de recurso depOnboardingSetting

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O depOnboardingSetting representa uma instância do serviço Apple DEP que está sendo integrado ao Intune. A instância de serviço integrada gerencia um token Apple usado para sincronizar dados entre o Apple e o Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|coleção [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Listar Propriedades e relações dos objetos [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Obter depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Leia as propriedades e as relações do objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Criar depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Criar um novo objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[Excluir depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-delete.md)|Nenhum|Exclui [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).|
|[Atualizar depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Atualiza as propriedades de um objeto [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md) .|
|[função getEncryptionPublicKey](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|String|Obter uma chave pública para usar para criptografar o token do programa de registro de dispositivo Apple|
|[Ação uploadDepToken](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|Nenhum|Carrega um novo token do programa de registro de dispositivos|
|[Ação syncWithAppleDeviceEnrollmentProgram](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|Nenhum|Sincroniza entre o programa de registro de dispositivo Apple e o Intune|
|[Ação shareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|Nenhum|Ainda não documentado|
|[Ação unshareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O UUID do objeto.|
|appleIdentifier|Cadeia de caracteres|A ID da Apple usada para obter o token atual.|
|tokenExpirationDateTime|DateTimeOffset|Quando o token expirará.|
|lastModifiedDateTime|DateTimeOffset|Quando o serviço foi integrado.|
|lastSuccessfulSyncDateTime|DateTimeOffset|Quando o serviço última syned com o Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Quando o Intune solicitou uma sincronização pela última vez.|
|shareTokenWithSchoolDataSyncService|Boolean|Se o compartilhamento de token DEP está ou não habilitado com o serviço de sincronização de dados da escola.|
|lastSyncErrorCode|Int32|Código de erro relatado pela Apple durante a última sincronização de Dep.|
|TokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|Obtém ou define o tipo de token Dep. Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.|
|tokenname|String|Nome amigável para token Dep|
|syncedDeviceCount|Int32|Obtém a contagem de dispositivos sincronizados|
|dataSharingConsentGranted|Boolean|Consentimento concedido para compartilhamento de dados com o serviço Apple Dep|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Perfil de registro iOS padrão|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Perfil de registro do MacOs padrão|
|enrollmentProfiles|coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Os perfis de registro.|
|importedAppleDeviceIdentities|coleção [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|As identidades importadas do dispositivo Apple.|

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
  "dataSharingConsentGranted": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




