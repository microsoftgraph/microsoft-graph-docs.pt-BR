---
title: Tipo de recurso androidDeviceOwnerEnrollmentProfile
description: Perfil de Registro usado para registrar dispositivos Enterprise Android usando o Gerenciamento de Nuvem do Google.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f88410522f63b289a2b2d6f55a2a1ebf85b46b5e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057653"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a>Tipo de recurso androidDeviceOwnerEnrollmentProfile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de Registro usado para registrar dispositivos Enterprise Android usando o Gerenciamento de Nuvem do Google.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidDeviceOwnerEnrollmentProfiles](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|[coleção androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Listar propriedades e relações dos objetos [androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|
|[Obter androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Leia propriedades e relações do [objeto androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|
|[Criar androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Crie um novo [objeto androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|
|[Excluir androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|Nenhum|Exclui um [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).|
|[Atualizar androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Atualize as propriedades de [um objeto androidDeviceOwnerEnrollmentProfile.](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|
|[Ação revokeToken](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|Nenhuma|Ainda não documentado|
|[Ação createToken](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accountId|String|GUID de locatário ao qual o perfil de registro pertence.|
|id|Cadeia de caracteres|GUID exclusivo do perfil de registro.|
|displayName|Cadeia de caracteres|Nome de exibição do perfil de registro.|
|description|Cadeia de caracteres|Descrição do perfil de registro.|
|enrollmentMode|[androidDeviceOwnerEnrollmentMode](../resources/intune-androidforwork-androiddeviceownerenrollmentmode.md)|O modo de registro de dispositivos que usam esse perfil de registro. Os valores possíveis são: `corporateOwnedDedicatedDevice`, `corporateOwnedFullyManaged`, `corporateOwnedWorkProfile`.|
|enrollmentTokenType|[androidDeviceOwnerEnrollmentTokenType](../resources/intune-androidforwork-androiddeviceownerenrollmenttokentype.md)|O tipo de token de registro para um perfil de registro. Os valores possíveis são: `default` e `corporateOwnedDedicatedDeviceWithAzureADSharedMode`.|
|createdDateTime|DateTimeOffset|Data e hora de criação do perfil de registro.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do perfil de registro.|
|tokenValue|String|Valor do token mais recentemente criado para este perfil de registro.|
|tokenCreationDateTime|DateTimeOffset|Data em que o token criado mais recentemente foi criado.|
|tokenExpirationDateTime|DateTimeOffset|Data e hora em que o token mais recentemente criado expirará.|
|enrolledDeviceCount|Int32|Número total de dispositivos Android que foram registrados usando esse perfil de registro.|
|qrCodeContent|String|Cadeia de caracteres usada para gerar um código QR para o token.|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Cadeia de caracteres usada para gerar um código QR para o token.|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Lista de marcas de escopo para esta instância entity.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "enrollmentMode": "String",
  "enrollmentTokenType": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
  "tokenCreationDateTime": "String (timestamp)",
  "tokenExpirationDateTime": "String (timestamp)",
  "enrolledDeviceCount": 1024,
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "roleScopeTagIds": [
    "String"
  ]
}
```



