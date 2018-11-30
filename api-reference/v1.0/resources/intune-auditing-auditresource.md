---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
ms.openlocfilehash: 452df4cb27dba5de04022c6ba7be08471286d866
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006427"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="b69aa-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="b69aa-103">auditResource resource type</span></span>

> <span data-ttu-id="b69aa-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b69aa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b69aa-105">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b69aa-105">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="b69aa-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b69aa-106">Properties</span></span>
|<span data-ttu-id="b69aa-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b69aa-107">Property</span></span>|<span data-ttu-id="b69aa-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b69aa-108">Type</span></span>|<span data-ttu-id="b69aa-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b69aa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b69aa-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b69aa-110">displayName</span></span>|<span data-ttu-id="b69aa-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b69aa-111">String</span></span>|<span data-ttu-id="b69aa-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b69aa-112">Display name.</span></span>|
|<span data-ttu-id="b69aa-113">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="b69aa-113">modifiedProperties</span></span>|<span data-ttu-id="b69aa-114">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b69aa-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="b69aa-115">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="b69aa-115">List of modified properties.</span></span>|
|<span data-ttu-id="b69aa-116">tipo</span><span class="sxs-lookup"><span data-stu-id="b69aa-116">type</span></span>|<span data-ttu-id="b69aa-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b69aa-117">String</span></span>|<span data-ttu-id="b69aa-118">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b69aa-118">Audit resource's type.</span></span>|
|<span data-ttu-id="b69aa-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="b69aa-119">resourceId</span></span>|<span data-ttu-id="b69aa-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b69aa-120">String</span></span>|<span data-ttu-id="b69aa-121">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="b69aa-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b69aa-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b69aa-122">Relationships</span></span>
<span data-ttu-id="b69aa-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b69aa-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b69aa-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b69aa-124">JSON Representation</span></span>
<span data-ttu-id="b69aa-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b69aa-125">Here is a JSON representation of the resource.</span></span>
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



