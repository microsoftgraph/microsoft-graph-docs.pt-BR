---
title: Tipo de recurso depOnboardingSetting
description: O depOnboardingSetting representa uma instância do serviço DEP da Apple que está sendo internado no Intune. A instância de serviço interna gerencia um Apple Token usado para sincronizar dados entre a Apple e o Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac9e8c7909d817544141a8a409d434c31d229ded5392376f51266b0532e221ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251243"
---
# <a name="deponboardingsetting-resource-type"></a>Tipo de recurso depOnboardingSetting

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O depOnboardingSetting representa uma instância do serviço DEP da Apple que está sendo internado no Intune. A instância de serviço interna gerencia um Apple Token usado para sincronizar dados entre a Apple e o Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar depOnboardingSettings](../api/intune-enrollment-deponboardingsetting-list.md)|[Coleção depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Listar propriedades e relações dos [objetos depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)|
|[Obter depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-get.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Leia propriedades e relações do objeto [depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)|
|[Criar depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-create.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Crie um novo [objeto depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)|
|[Excluir depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-delete.md)|Nenhum|Exclui um [depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md).|
|[Atualizar depOnboardingSetting](../api/intune-enrollment-deponboardingsetting-update.md)|[depOnboardingSetting](../resources/intune-enrollment-deponboardingsetting.md)|Atualize as propriedades [de um objeto depOnboardingSetting.](../resources/intune-enrollment-deponboardingsetting.md)|
|[função getEncryptionPublicKey](../api/intune-enrollment-deponboardingsetting-getencryptionpublickey.md)|Cadeia de caracteres|Obter uma chave pública a ser usada para criptografar o token de programa de registro de dispositivo Apple|
|[ação generateEncryptionPublicKey](../api/intune-enrollment-deponboardingsetting-generateencryptionpublickey.md)|Cadeia de caracteres|Gerar uma chave pública a ser usada para criptografar o token de programa de registro de dispositivo Apple|
|[Ação uploadDepToken](../api/intune-enrollment-deponboardingsetting-uploaddeptoken.md)|Nenhum|Carrega um novo token do Programa de Registro de Dispositivo|
|[Ação syncWithAppleDeviceEnrollmentProgram](../api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram.md)|Nenhum|Sincroniza entre o Programa de Registro de Dispositivo Apple e o Intune|
|[Ação shareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice.md)|Nenhuma|Ainda não documentado|
|[Ação unshareForSchoolDataSyncService](../api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice.md)|Nenhuma|Ainda não documentado|
|[função getExpiringVppTokenCount](../api/intune-enrollment-deponboardingsetting-getexpiringvpptokencount.md)|Int32|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O UUID do objeto.|
|appleIdentifier|Cadeia de caracteres|A ID da Apple usada para obter o token atual.|
|tokenExpirationDateTime|DateTimeOffset|Quando o token expirar.|
|lastModifiedDateTime|DateTimeOffset|Quando o serviço foi integrado.|
|lastSuccessfulSyncDateTime|DateTimeOffset|Quando o serviço foi sintetizado pela última vez com o Intune|
|lastSyncTriggeredDateTime|DateTimeOffset|Quando o Intune solicitou pela última vez uma sincronização.|
|shareTokenWithSchoolDataSyncService|Boolean|Se o compartilhamento de token Dep está habilitado ou não com o School Data Sync serviço.|
|lastSyncErrorCode|Int32|Código de erro relatado pela Apple durante a última sincronização de dep.|
|tokenType|[depTokenType](../resources/intune-enrollment-deptokentype.md)|Obtém ou define o Tipo de Token de Dep. Os valores possíveis são: `none`, `dep`, `appleSchoolManager`.|
|tokenName|Cadeia de caracteres|Nome amigável para Token de Dep|
|syncedDeviceCount|Int32|Obtém contagem de dispositivos sincronizados|
|dataSharingConsentGranted|Boolean|Consentimento concedido para compartilhamento de dados com o Serviço de Dep da Apple|
|roleScopeTagIds|String collection|Lista de marcas de escopo para esta instância entity.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|defaultIosEnrollmentProfile|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Perfil de Registro padrão do iOS|
|defaultMacOsEnrollmentProfile|[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)|Perfil de Registro padrão de MacOs|
|enrollmentProfiles|[Coleção enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Os perfis de registro.|
|importedAppleDeviceIdentities|[Coleção importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)|As identidades de dispositivo Apple importadas.|

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




