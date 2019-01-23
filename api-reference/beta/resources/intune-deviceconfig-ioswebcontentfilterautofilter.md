---
title: tipo de recurso de iosWebContentFilterAutoFilter
description: Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS. Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5be275b74e2675881b9d36b047e2017ef95adb2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401226"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="0c061-104">tipo de recurso de iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="0c061-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="0c061-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0c061-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c061-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0c061-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c061-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0c061-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c061-108">Representa um tipo de configuração de filtro de conteúdo da Web, que habilita o recurso de filtro automático iOS e permite que o controle de acesso de URL adicional iOS.</span><span class="sxs-lookup"><span data-stu-id="0c061-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="0c061-109">Quando construída sem valores de propriedade, o dispositivo iOS permitirá o filtro automático independentemente.</span><span class="sxs-lookup"><span data-stu-id="0c061-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="0c061-110">Herda de [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="0c061-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c061-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c061-111">Properties</span></span>
|<span data-ttu-id="0c061-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c061-112">Property</span></span>|<span data-ttu-id="0c061-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c061-113">Type</span></span>|<span data-ttu-id="0c061-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c061-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c061-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="0c061-115">allowedUrls</span></span>|<span data-ttu-id="0c061-116">String collection</span><span class="sxs-lookup"><span data-stu-id="0c061-116">String collection</span></span>|<span data-ttu-id="0c061-117">URLs adicionais permitidos para o access</span><span class="sxs-lookup"><span data-stu-id="0c061-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="0c061-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="0c061-118">blockedUrls</span></span>|<span data-ttu-id="0c061-119">String collection</span><span class="sxs-lookup"><span data-stu-id="0c061-119">String collection</span></span>|<span data-ttu-id="0c061-120">URLs adicionais bloqueados para acesso</span><span class="sxs-lookup"><span data-stu-id="0c061-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c061-121">Relações</span><span class="sxs-lookup"><span data-stu-id="0c061-121">Relationships</span></span>
<span data-ttu-id="0c061-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c061-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c061-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c061-123">JSON Representation</span></span>
<span data-ttu-id="0c061-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c061-124">Here is a JSON representation of the resource.</span></span>
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




