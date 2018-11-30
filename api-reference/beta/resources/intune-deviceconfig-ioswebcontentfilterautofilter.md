---
title: tipo de recurso de iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS. Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.
ms.openlocfilehash: 04a221ac512ab3934702a2a9e3178ba23a2ac3ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038744"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="fbc2e-104">tipo de recurso de iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="fbc2e-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="fbc2e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbc2e-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbc2e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbc2e-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbc2e-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fbc2e-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbc2e-108">Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS.</span><span class="sxs-lookup"><span data-stu-id="fbc2e-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="fbc2e-109">Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.</span><span class="sxs-lookup"><span data-stu-id="fbc2e-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>

<span data-ttu-id="fbc2e-110">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="fbc2e-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbc2e-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbc2e-111">Properties</span></span>
|<span data-ttu-id="fbc2e-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbc2e-112">Property</span></span>|<span data-ttu-id="fbc2e-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc2e-113">Type</span></span>|<span data-ttu-id="fbc2e-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc2e-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc2e-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="fbc2e-115">allowedUrls</span></span>|<span data-ttu-id="fbc2e-116">String collection</span><span class="sxs-lookup"><span data-stu-id="fbc2e-116">String collection</span></span>|<span data-ttu-id="fbc2e-117">URLs adicionais permitidos para o access</span><span class="sxs-lookup"><span data-stu-id="fbc2e-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="fbc2e-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="fbc2e-118">blockedUrls</span></span>|<span data-ttu-id="fbc2e-119">String collection</span><span class="sxs-lookup"><span data-stu-id="fbc2e-119">String collection</span></span>|<span data-ttu-id="fbc2e-120">URLs adicionais bloqueados para acesso</span><span class="sxs-lookup"><span data-stu-id="fbc2e-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbc2e-121">Relações</span><span class="sxs-lookup"><span data-stu-id="fbc2e-121">Relationships</span></span>
<span data-ttu-id="fbc2e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbc2e-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbc2e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbc2e-123">JSON Representation</span></span>
<span data-ttu-id="fbc2e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbc2e-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```





