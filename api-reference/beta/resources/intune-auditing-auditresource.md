---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20c39cc5138be5c731bc34b1e13f8536e7581c40
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558304"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="3f55d-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="3f55d-103">auditResource resource type</span></span>

> <span data-ttu-id="3f55d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f55d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f55d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f55d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f55d-106">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="3f55d-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="3f55d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f55d-107">Properties</span></span>
|<span data-ttu-id="3f55d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f55d-108">Property</span></span>|<span data-ttu-id="3f55d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f55d-109">Type</span></span>|<span data-ttu-id="3f55d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f55d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f55d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3f55d-111">displayName</span></span>|<span data-ttu-id="3f55d-112">String</span><span class="sxs-lookup"><span data-stu-id="3f55d-112">String</span></span>|<span data-ttu-id="3f55d-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="3f55d-113">Display name.</span></span>|
|<span data-ttu-id="3f55d-114">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="3f55d-114">modifiedProperties</span></span>|<span data-ttu-id="3f55d-115">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="3f55d-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="3f55d-116">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="3f55d-116">List of modified properties.</span></span>|
|<span data-ttu-id="3f55d-117">type</span><span class="sxs-lookup"><span data-stu-id="3f55d-117">type</span></span>|<span data-ttu-id="3f55d-118">String</span><span class="sxs-lookup"><span data-stu-id="3f55d-118">String</span></span>|<span data-ttu-id="3f55d-119">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="3f55d-119">Audit resource's type.</span></span>|
|<span data-ttu-id="3f55d-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="3f55d-120">resourceId</span></span>|<span data-ttu-id="3f55d-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f55d-121">String</span></span>|<span data-ttu-id="3f55d-122">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="3f55d-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f55d-123">Relações</span><span class="sxs-lookup"><span data-stu-id="3f55d-123">Relationships</span></span>
<span data-ttu-id="3f55d-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f55d-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f55d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f55d-125">JSON Representation</span></span>
<span data-ttu-id="3f55d-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f55d-126">Here is a JSON representation of the resource.</span></span>
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





