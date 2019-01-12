---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac7da99203631696b8c93fbde62db906143ffe38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952241"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="421bd-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="421bd-103">auditResource resource type</span></span>

> <span data-ttu-id="421bd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="421bd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="421bd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="421bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="421bd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="421bd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="421bd-107">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="421bd-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="421bd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="421bd-108">Properties</span></span>
|<span data-ttu-id="421bd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="421bd-109">Property</span></span>|<span data-ttu-id="421bd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="421bd-110">Type</span></span>|<span data-ttu-id="421bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="421bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="421bd-112">displayName</span><span class="sxs-lookup"><span data-stu-id="421bd-112">displayName</span></span>|<span data-ttu-id="421bd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="421bd-113">String</span></span>|<span data-ttu-id="421bd-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="421bd-114">Display name.</span></span>|
|<span data-ttu-id="421bd-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="421bd-115">modifiedProperties</span></span>|<span data-ttu-id="421bd-116">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="421bd-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="421bd-117">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="421bd-117">List of modified properties.</span></span>|
|<span data-ttu-id="421bd-118">tipo</span><span class="sxs-lookup"><span data-stu-id="421bd-118">type</span></span>|<span data-ttu-id="421bd-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="421bd-119">String</span></span>|<span data-ttu-id="421bd-120">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="421bd-120">Audit resource's type.</span></span>|
|<span data-ttu-id="421bd-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="421bd-121">resourceId</span></span>|<span data-ttu-id="421bd-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="421bd-122">String</span></span>|<span data-ttu-id="421bd-123">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="421bd-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="421bd-124">Relações</span><span class="sxs-lookup"><span data-stu-id="421bd-124">Relationships</span></span>
<span data-ttu-id="421bd-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="421bd-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="421bd-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="421bd-126">JSON Representation</span></span>
<span data-ttu-id="421bd-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="421bd-127">Here is a JSON representation of the resource.</span></span>
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





