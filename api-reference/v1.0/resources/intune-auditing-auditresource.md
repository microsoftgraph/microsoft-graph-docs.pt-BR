---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e2a6b2309e831a872c4cde04a951819cac292ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534343"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="53570-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="53570-103">auditResource resource type</span></span>

> <span data-ttu-id="53570-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53570-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53570-105">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="53570-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="53570-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53570-106">Properties</span></span>
|<span data-ttu-id="53570-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53570-107">Property</span></span>|<span data-ttu-id="53570-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="53570-108">Type</span></span>|<span data-ttu-id="53570-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="53570-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53570-110">displayName</span><span class="sxs-lookup"><span data-stu-id="53570-110">displayName</span></span>|<span data-ttu-id="53570-111">String</span><span class="sxs-lookup"><span data-stu-id="53570-111">String</span></span>|<span data-ttu-id="53570-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="53570-112">Display name.</span></span>|
|<span data-ttu-id="53570-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="53570-113">modifiedProperties</span></span>|<span data-ttu-id="53570-114">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="53570-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="53570-115">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="53570-115">List of modified properties.</span></span>|
|<span data-ttu-id="53570-116">type</span><span class="sxs-lookup"><span data-stu-id="53570-116">type</span></span>|<span data-ttu-id="53570-117">String</span><span class="sxs-lookup"><span data-stu-id="53570-117">String</span></span>|<span data-ttu-id="53570-118">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="53570-118">Audit resource's type.</span></span>|
|<span data-ttu-id="53570-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="53570-119">resourceId</span></span>|<span data-ttu-id="53570-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53570-120">String</span></span>|<span data-ttu-id="53570-121">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="53570-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53570-122">Relações</span><span class="sxs-lookup"><span data-stu-id="53570-122">Relationships</span></span>
<span data-ttu-id="53570-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53570-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53570-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53570-124">JSON Representation</span></span>
<span data-ttu-id="53570-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53570-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```



