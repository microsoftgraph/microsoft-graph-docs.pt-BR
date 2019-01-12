---
title: tipo de recurso de androidDeviceOwnerEnrollmentProfile
description: Perfil de registro usado para registrar dispositivos COSU usando o Gerenciamento de Nuvem do Google.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 5e609f16978f3dd68eb680692149954f83e6cc6d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963553"
---
# <a name="androiddeviceownerenrollmentprofile-resource-type"></a>tipo de recurso de androidDeviceOwnerEnrollmentProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Perfil de registro usado para registrar dispositivos COSU usando o Gerenciamento de Nuvem do Google.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista androidDeviceOwnerEnrollmentProfiles](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-list.md)|coleção [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Lista as propriedades e os relacionamentos dos objetos [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .|
|[Obter androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-get.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Leia as propriedades e os relacionamentos do objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .|
|[Criar androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-create.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Crie um novo objeto de [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .|
|[Excluir androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-delete.md)|Nenhum|Exclui um [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).|
|[Atualizar androidDeviceOwnerEnrollmentProfile](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-update.md)|[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)|Atualize as propriedades de um objeto [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) .|
|[Ação revokeToken](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken.md)|Nenhuma|Ainda não documentado|
|[Ação createToken](../api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken.md)|Nenhuma|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accountId|String|GUID de locatário ao qual o perfil de registro pertence.|
|id|String|GUID exclusivo do perfil de registro.|
|displayName|String|Nome de exibição do perfil de registro.|
|description|String|Descrição do perfil de registro.|
|createdDateTime|DateTimeOffset|Data e hora de criação do perfil de registro.|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do perfil de registro.|
|tokenValue|String|Valor do token mais recentemente criado para este perfil de registro.|
|tokenCreationDateTime|DateTimeOffset|Data hora em que o token mais recentemente criado foi criado.|
|tokenExpirationDateTime|DateTimeOffset|Data e hora em que o token mais recentemente criado expirará.|
|enrolledDeviceCount|Int32|Número total de dispositivos Android que foram registrados usando esse perfil de registro.|
|qrCodeContent|String|Cadeia de caracteres usada para gerar um código QR para o token.|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Cadeia de caracteres usada para gerar um código QR para o token.|

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
  }
}
```





