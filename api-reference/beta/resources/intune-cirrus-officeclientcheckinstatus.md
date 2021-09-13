---
title: Tipo de recurso officeClientCheckinStatus
description: Entidade que descreve as estatísticas de check-in do locatário.
ms.localizationpriority: medium
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 416b7f20477109718ab8b2efd26190050d910fda
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064424"
---
# <a name="officeclientcheckinstatus-resource-type"></a>Tipo de recurso officeClientCheckinStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que descreve as estatísticas de check-in do locatário.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário usando o dispositivo.|
|deviceName|String|Nome do dispositivo tentando fazer check-in.|
|devicePlatform|Cadeia de caracteres|Plataforma de dispositivo tentando fazer check-in.|
|devicePlatformVersion|Cadeia de Caracteres|Versão da plataforma do dispositivo tentando fazer check-in.|
|wasSuccessful|Boolean|Se a última verificação tiver sido bem-sucedida.|
|userId|Cadeia de caracteres|Identificador de usuário usando o dispositivo.|
|checkinDateTime|DateTimeOffset|Última hora de check-in do dispositivo em UTC.|
|errorMessage|Cadeia de caracteres|Mensagem de erro se alguma associada ao último check-in.|
|appliedPolicies|Conjunto de cadeias de caracteres|Lista de políticas entregues ao dispositivo como última verificação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



