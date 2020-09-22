---
title: tipo de recurso roleScopeTagInfo
description: Uma classe que contém as propriedades do objeto de marca de escopo de função.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67927894be0f4209e915781169a45d5daa874b20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076236"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="44595-103">tipo de recurso roleScopeTagInfo</span><span class="sxs-lookup"><span data-stu-id="44595-103">roleScopeTagInfo resource type</span></span>

<span data-ttu-id="44595-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44595-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44595-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44595-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44595-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44595-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44595-107">Uma classe que contém as propriedades do objeto de marca de escopo de função.</span><span class="sxs-lookup"><span data-stu-id="44595-107">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="44595-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44595-108">Properties</span></span>
|<span data-ttu-id="44595-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44595-109">Property</span></span>|<span data-ttu-id="44595-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="44595-110">Type</span></span>|<span data-ttu-id="44595-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="44595-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44595-112">displayName</span><span class="sxs-lookup"><span data-stu-id="44595-112">displayName</span></span>|<span data-ttu-id="44595-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44595-113">String</span></span>|<span data-ttu-id="44595-114">Nome de exibição da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="44595-114">Scope Tag Display name.</span></span>|
|<span data-ttu-id="44595-115">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="44595-115">roleScopeTagId</span></span>|<span data-ttu-id="44595-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44595-116">String</span></span>|<span data-ttu-id="44595-117">ID da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="44595-117">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44595-118">Relações</span><span class="sxs-lookup"><span data-stu-id="44595-118">Relationships</span></span>
<span data-ttu-id="44595-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44595-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44595-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44595-120">JSON Representation</span></span>
<span data-ttu-id="44595-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44595-121">Here is a JSON representation of the resource.</span></span>
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






