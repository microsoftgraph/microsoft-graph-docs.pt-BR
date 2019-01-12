---
title: tipo de recurso de iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS. Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 03e3c4f51e673be1e2bada89e06a26048fe4e385
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916774"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="4b3d6-104">tipo de recurso de iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="4b3d6-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="4b3d6-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4b3d6-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b3d6-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4b3d6-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b3d6-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4b3d6-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b3d6-108">Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS.</span><span class="sxs-lookup"><span data-stu-id="4b3d6-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="4b3d6-109">Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.</span><span class="sxs-lookup"><span data-stu-id="4b3d6-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>

<span data-ttu-id="4b3d6-110">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="4b3d6-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b3d6-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b3d6-111">Properties</span></span>
|<span data-ttu-id="4b3d6-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b3d6-112">Property</span></span>|<span data-ttu-id="4b3d6-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b3d6-113">Type</span></span>|<span data-ttu-id="4b3d6-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b3d6-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b3d6-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="4b3d6-115">allowedUrls</span></span>|<span data-ttu-id="4b3d6-116">String collection</span><span class="sxs-lookup"><span data-stu-id="4b3d6-116">String collection</span></span>|<span data-ttu-id="4b3d6-117">URLs adicionais permitidos para o access</span><span class="sxs-lookup"><span data-stu-id="4b3d6-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="4b3d6-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="4b3d6-118">blockedUrls</span></span>|<span data-ttu-id="4b3d6-119">String collection</span><span class="sxs-lookup"><span data-stu-id="4b3d6-119">String collection</span></span>|<span data-ttu-id="4b3d6-120">URLs adicionais bloqueados para acesso</span><span class="sxs-lookup"><span data-stu-id="4b3d6-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b3d6-121">Relações</span><span class="sxs-lookup"><span data-stu-id="4b3d6-121">Relationships</span></span>
<span data-ttu-id="4b3d6-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4b3d6-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b3d6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b3d6-123">JSON Representation</span></span>
<span data-ttu-id="4b3d6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b3d6-124">Here is a JSON representation of the resource.</span></span>
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





