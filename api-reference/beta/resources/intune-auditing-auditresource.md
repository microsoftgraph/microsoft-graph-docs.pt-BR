---
title: Tipo de recurso auditResource
description: Uma classe que contém as propriedades para o Recurso de auditoria.
author: tfitzmac
ms.openlocfilehash: c60c76f899fabfbced271e6ec38043337b8b3851
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339862"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="83780-103">Tipo de recurso auditResource</span><span class="sxs-lookup"><span data-stu-id="83780-103">auditResource resource type</span></span>

> <span data-ttu-id="83780-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="83780-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83780-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="83780-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83780-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="83780-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83780-107">Uma classe que contém as propriedades para o Recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="83780-107">A class containing the properties for Audit Resource.</span></span>
## <a name="properties"></a><span data-ttu-id="83780-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83780-108">Properties</span></span>
|<span data-ttu-id="83780-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83780-109">Property</span></span>|<span data-ttu-id="83780-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="83780-110">Type</span></span>|<span data-ttu-id="83780-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83780-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83780-112">displayName</span><span class="sxs-lookup"><span data-stu-id="83780-112">displayName</span></span>|<span data-ttu-id="83780-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83780-113">String</span></span>|<span data-ttu-id="83780-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="83780-114">Display name.</span></span>|
|<span data-ttu-id="83780-115">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="83780-115">modifiedProperties</span></span>|<span data-ttu-id="83780-116">Conjunto [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="83780-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="83780-117">Lista de propriedades modificadas.</span><span class="sxs-lookup"><span data-stu-id="83780-117">List of modified properties.</span></span>|
|<span data-ttu-id="83780-118">tipo</span><span class="sxs-lookup"><span data-stu-id="83780-118">type</span></span>|<span data-ttu-id="83780-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83780-119">String</span></span>|<span data-ttu-id="83780-120">Tipo de recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="83780-120">Audit resource's type.</span></span>|
|<span data-ttu-id="83780-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="83780-121">resourceId</span></span>|<span data-ttu-id="83780-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="83780-122">String</span></span>|<span data-ttu-id="83780-123">ID do recurso de auditoria.</span><span class="sxs-lookup"><span data-stu-id="83780-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83780-124">Relações</span><span class="sxs-lookup"><span data-stu-id="83780-124">Relationships</span></span>
<span data-ttu-id="83780-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83780-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="83780-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83780-126">JSON Representation</span></span>
<span data-ttu-id="83780-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83780-127">Here is a JSON representation of the resource.</span></span>
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





