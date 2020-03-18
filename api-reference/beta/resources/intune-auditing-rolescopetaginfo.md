---
title: tipo de recurso roleScopeTagInfo
description: Uma classe que contém as propriedades do objeto de marca de escopo de função.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c932a1353f684771a1979ae970141d674f726142
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797406"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="49e69-103">tipo de recurso roleScopeTagInfo</span><span class="sxs-lookup"><span data-stu-id="49e69-103">roleScopeTagInfo resource type</span></span>

> <span data-ttu-id="49e69-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="49e69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49e69-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="49e69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49e69-106">Uma classe que contém as propriedades do objeto de marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="49e69-106">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="49e69-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49e69-107">Properties</span></span>
|<span data-ttu-id="49e69-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49e69-108">Property</span></span>|<span data-ttu-id="49e69-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="49e69-109">Type</span></span>|<span data-ttu-id="49e69-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="49e69-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49e69-111">displayName</span><span class="sxs-lookup"><span data-stu-id="49e69-111">displayName</span></span>|<span data-ttu-id="49e69-112">String</span><span class="sxs-lookup"><span data-stu-id="49e69-112">String</span></span>|<span data-ttu-id="49e69-113">Nome de exibição da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="49e69-113">Scope Tag Display name.</span></span>|
|<span data-ttu-id="49e69-114">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="49e69-114">roleScopeTagId</span></span>|<span data-ttu-id="49e69-115">String</span><span class="sxs-lookup"><span data-stu-id="49e69-115">String</span></span>|<span data-ttu-id="49e69-116">ID da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="49e69-116">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49e69-117">Relações</span><span class="sxs-lookup"><span data-stu-id="49e69-117">Relationships</span></span>
<span data-ttu-id="49e69-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="49e69-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49e69-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49e69-119">JSON Representation</span></span>
<span data-ttu-id="49e69-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49e69-120">Here is a JSON representation of the resource.</span></span>
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



