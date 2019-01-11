---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bf1d7881c7028e14a048d3f286f684f26393ab58
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807004"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="fc5de-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="fc5de-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="fc5de-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fc5de-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc5de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fc5de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc5de-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fc5de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc5de-107">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="fc5de-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="fc5de-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc5de-108">Properties</span></span>
|<span data-ttu-id="fc5de-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc5de-109">Property</span></span>|<span data-ttu-id="fc5de-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc5de-110">Type</span></span>|<span data-ttu-id="fc5de-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc5de-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc5de-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fc5de-112">displayName</span></span>|<span data-ttu-id="fc5de-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fc5de-113">String</span></span>|<span data-ttu-id="fc5de-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="fc5de-114">Display name</span></span>|
|<span data-ttu-id="fc5de-115">recursos</span><span class="sxs-lookup"><span data-stu-id="fc5de-115">resources</span></span>|<span data-ttu-id="fc5de-116">String collection</span><span class="sxs-lookup"><span data-stu-id="fc5de-116">String collection</span></span>|<span data-ttu-id="fc5de-117">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="fc5de-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc5de-118">Relações</span><span class="sxs-lookup"><span data-stu-id="fc5de-118">Relationships</span></span>
<span data-ttu-id="fc5de-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc5de-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc5de-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc5de-120">JSON Representation</span></span>
<span data-ttu-id="fc5de-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc5de-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```





