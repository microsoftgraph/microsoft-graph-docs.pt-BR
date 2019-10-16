---
title: tipo de recurso scopeTagInfo
description: Uma classe que contém as propriedades do objeto de marca de escopo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8238881d8a14cb8aa1dfcc01031105be0069c21
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538501"
---
# <a name="scopetaginfo-resource-type"></a><span data-ttu-id="078cd-103">tipo de recurso scopeTagInfo</span><span class="sxs-lookup"><span data-stu-id="078cd-103">scopeTagInfo resource type</span></span>

> <span data-ttu-id="078cd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="078cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="078cd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="078cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="078cd-106">Uma classe que contém as propriedades do objeto de marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="078cd-106">A class containing the properties of Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="078cd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="078cd-107">Properties</span></span>
|<span data-ttu-id="078cd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="078cd-108">Property</span></span>|<span data-ttu-id="078cd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="078cd-109">Type</span></span>|<span data-ttu-id="078cd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="078cd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="078cd-111">scopeTagName</span><span class="sxs-lookup"><span data-stu-id="078cd-111">scopeTagName</span></span>|<span data-ttu-id="078cd-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="078cd-112">String</span></span>|<span data-ttu-id="078cd-113">Nome de exibição da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="078cd-113">Scope Tag Display name.</span></span>|
|<span data-ttu-id="078cd-114">scopeTagId</span><span class="sxs-lookup"><span data-stu-id="078cd-114">scopeTagId</span></span>|<span data-ttu-id="078cd-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="078cd-115">String</span></span>|<span data-ttu-id="078cd-116">ID da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="078cd-116">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="078cd-117">Relações</span><span class="sxs-lookup"><span data-stu-id="078cd-117">Relationships</span></span>
<span data-ttu-id="078cd-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="078cd-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="078cd-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="078cd-119">JSON Representation</span></span>
<span data-ttu-id="078cd-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="078cd-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scopeTagInfo",
  "scopeTagName": "String",
  "scopeTagId": "String"
}
```



