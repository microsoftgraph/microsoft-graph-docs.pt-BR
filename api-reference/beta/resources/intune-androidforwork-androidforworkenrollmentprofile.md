---
title: Tipo de recurso androidForWorkEnrollmentProfile
description: Perfil de registro usado para registrar dispositivos COSU usando o Gerenciamento de Nuvem do Google.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1cf839526d54dc0bc157254ed4817075af7c3b64
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409640"
---
# <a name="androidforworkenrollmentprofile-resource-type"></a>Tipo de recurso androidForWorkEnrollmentProfile

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Perfil de registro usado para registrar dispositivos COSU usando o Gerenciamento de Nuvem do Google.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidForWorkEnrollmentProfiles](../api/intune-androidforwork-androidforworkenrollmentprofile-list.md)|Coleção [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Lista propriedades e relações dos objetos [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Obter androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-get.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Propriedades de leitura e relações do objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Criar androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-create.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Cria um novo objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Excluir androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-delete.md)|Nenhuma|Exclui um [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Atualizar androidForWorkEnrollmentProfile](../api/intune-androidforwork-androidforworkenrollmentprofile-update.md)|[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md)|Atualiza as propriedades de um objeto [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md).|
|[Ação revokeToken](../api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken.md)|Nenhuma|Ainda não documentado|
|[Ação createToken](../api/intune-androidforwork-androidforworkenrollmentprofile-createtoken.md)|Nenhuma|Ainda não documentado|

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
  "@odata.type": "microsoft.graph.androidForWorkEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "tokenValue": "String",
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




