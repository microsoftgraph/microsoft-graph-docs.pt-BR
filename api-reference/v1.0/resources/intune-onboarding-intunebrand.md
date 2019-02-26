---
title: Tipo de recurso intuneBrand
description: intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a47e19aaca3aa5e7469d9fb01cbae7b5363c1270
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257453"
---
# <a name="intunebrand-resource-type"></a>Tipo de recurso intuneBrand

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

intuneBrand contém dados que são usados na personalização da aparência dos aplicativos do Portal da Empresa, bem como do portal da Web de usuários finais.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome da empresa/organização exibido para usuários finais.|
|contactITName|String|Nome da pessoa/organização responsável pelo suporte de TI.|
|contactITPhoneNumber|String|Número de telefone da pessoa/organização responsável pelo suporte de TI.|
|contactITEmailAddress|String|Endereço de email da pessoa/organização responsável pelo suporte de TI.|
|contactITNotes|String|Comentários de texto relacionados à pessoa/organização responsável pelo suporte de TI.|
|privacyUrl|String|URL da política de privacidade da empresa/organização.|
|onlineSupportSiteUrl|String|URL do site de assistência técnica de TI da empresa/organização.|
|onlineSupportSiteName|Cadeia de caracteres|Nome de exibição do site de assistência técnica de TI da empresa/organização.|
|themeColor|[rgbColor](../resources/intune-onboarding-rgbcolor.md)|Cor de tema principal usado nos aplicativos e no portal da Web do Portal da Empresa.|
|showLogo|Boolean|Booliano que indica se as imagens de logotipo fornecidas pelo administrador serão exibidas ou não.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo claro atrás do logotipo.|
|darkBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Imagem do logotipo exibida nos aplicativos do Portal da Empresa que têm um plano de fundo escuro atrás do logotipo.|
|showNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.|
|showDisplayNameNextToLogo|Booliano|Booliano que indica se o nome de exibição fornecido pelo administrador será exibido ao lado da imagem do logotipo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "showDisplayNameNextToLogo": true
}
```



