---
title: Tipo de recurso cloudPcUserRoleScopeTagInfo
description: Representa as informações da marca de escopo com nome de exibição e identidade.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61df383dca51ec2494eb10b745bc227bcfc5d9b8
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211183"
---
# <a name="cloudpcuserrolescopetaginfo-resource-type"></a><span data-ttu-id="7ca1b-103">Tipo de recurso cloudPcUserRoleScopeTagInfo</span><span class="sxs-lookup"><span data-stu-id="7ca1b-103">cloudPcUserRoleScopeTagInfo resource type</span></span>

<span data-ttu-id="7ca1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ca1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ca1b-105">Representa as informações da marca de escopo com nome de exibição e identidade.</span><span class="sxs-lookup"><span data-stu-id="7ca1b-105">Represents the scope tag info with display name and identity.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="7ca1b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ca1b-106">Properties</span></span>
|<span data-ttu-id="7ca1b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ca1b-107">Property</span></span>|<span data-ttu-id="7ca1b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ca1b-108">Type</span></span>|<span data-ttu-id="7ca1b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ca1b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ca1b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7ca1b-110">displayName</span></span>|<span data-ttu-id="7ca1b-111">String</span><span class="sxs-lookup"><span data-stu-id="7ca1b-111">String</span></span>|<span data-ttu-id="7ca1b-112">Nome de exibição da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="7ca1b-112">Scope tag display name.</span></span>|
|<span data-ttu-id="7ca1b-113">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="7ca1b-113">roleScopeTagId</span></span>|<span data-ttu-id="7ca1b-114">String</span><span class="sxs-lookup"><span data-stu-id="7ca1b-114">String</span></span>|<span data-ttu-id="7ca1b-115">ID da marca de escopo.</span><span class="sxs-lookup"><span data-stu-id="7ca1b-115">Scope tag ID.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ca1b-116">Relações</span><span class="sxs-lookup"><span data-stu-id="7ca1b-116">Relationships</span></span>

<span data-ttu-id="7ca1b-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ca1b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ca1b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ca1b-118">JSON Representation</span></span>
<span data-ttu-id="7ca1b-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ca1b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserRoleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```