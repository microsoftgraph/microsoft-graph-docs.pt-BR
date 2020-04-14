---
title: tipo de recurso roleScopeTagInfo
description: Uma classe que contém as propriedades do objeto de marca de escopo de função.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7240e06e34d003eceeece5c8b7fbb365ed20bf1f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441210"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="61fa2-103">tipo de recurso roleScopeTagInfo</span><span class="sxs-lookup"><span data-stu-id="61fa2-103">roleScopeTagInfo resource type</span></span>

<span data-ttu-id="61fa2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61fa2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61fa2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61fa2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61fa2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61fa2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61fa2-107">Uma classe que contém as propriedades do objeto de marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="61fa2-107">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="61fa2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="61fa2-108">Properties</span></span>
|<span data-ttu-id="61fa2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61fa2-109">Property</span></span>|<span data-ttu-id="61fa2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="61fa2-110">Type</span></span>|<span data-ttu-id="61fa2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="61fa2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61fa2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="61fa2-112">displayName</span></span>|<span data-ttu-id="61fa2-113">String</span><span class="sxs-lookup"><span data-stu-id="61fa2-113">String</span></span>|<span data-ttu-id="61fa2-114">Nome de exibição da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="61fa2-114">Scope Tag Display name.</span></span>|
|<span data-ttu-id="61fa2-115">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="61fa2-115">roleScopeTagId</span></span>|<span data-ttu-id="61fa2-116">String</span><span class="sxs-lookup"><span data-stu-id="61fa2-116">String</span></span>|<span data-ttu-id="61fa2-117">ID da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="61fa2-117">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61fa2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="61fa2-118">Relationships</span></span>
<span data-ttu-id="61fa2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61fa2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61fa2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="61fa2-120">JSON Representation</span></span>
<span data-ttu-id="61fa2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="61fa2-121">Here is a JSON representation of the resource.</span></span>
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



