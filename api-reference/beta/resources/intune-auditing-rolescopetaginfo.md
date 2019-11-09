---
title: tipo de recurso roleScopeTagInfo
description: Uma classe que contém as propriedades do objeto de marca de escopo de função.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 09ddd40d5f24b6c85c3637960a446728830e8dea
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38082659"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="4ff0d-103">tipo de recurso roleScopeTagInfo</span><span class="sxs-lookup"><span data-stu-id="4ff0d-103">roleScopeTagInfo resource type</span></span>

> <span data-ttu-id="4ff0d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ff0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ff0d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ff0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ff0d-106">Uma classe que contém as propriedades do objeto de marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="4ff0d-106">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="4ff0d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ff0d-107">Properties</span></span>
|<span data-ttu-id="4ff0d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ff0d-108">Property</span></span>|<span data-ttu-id="4ff0d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ff0d-109">Type</span></span>|<span data-ttu-id="4ff0d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ff0d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ff0d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4ff0d-111">displayName</span></span>|<span data-ttu-id="4ff0d-112">String</span><span class="sxs-lookup"><span data-stu-id="4ff0d-112">String</span></span>|<span data-ttu-id="4ff0d-113">Nome de exibição da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="4ff0d-113">Scope Tag Display name.</span></span>|
|<span data-ttu-id="4ff0d-114">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="4ff0d-114">roleScopeTagId</span></span>|<span data-ttu-id="4ff0d-115">String</span><span class="sxs-lookup"><span data-stu-id="4ff0d-115">String</span></span>|<span data-ttu-id="4ff0d-116">ID da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="4ff0d-116">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ff0d-117">Relações</span><span class="sxs-lookup"><span data-stu-id="4ff0d-117">Relationships</span></span>
<span data-ttu-id="4ff0d-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ff0d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ff0d-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ff0d-119">JSON Representation</span></span>
<span data-ttu-id="4ff0d-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ff0d-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```



