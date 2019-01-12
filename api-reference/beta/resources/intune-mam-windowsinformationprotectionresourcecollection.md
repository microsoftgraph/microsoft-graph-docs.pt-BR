---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a65704170c048f4aae66876f11ef8543c7b09e2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933005"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="a8a4b-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="a8a4b-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="a8a4b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a8a4b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8a4b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a8a4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8a4b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a8a4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8a4b-107">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="a8a4b-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="a8a4b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8a4b-108">Properties</span></span>
|<span data-ttu-id="a8a4b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8a4b-109">Property</span></span>|<span data-ttu-id="a8a4b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8a4b-110">Type</span></span>|<span data-ttu-id="a8a4b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8a4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8a4b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a8a4b-112">displayName</span></span>|<span data-ttu-id="a8a4b-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a8a4b-113">String</span></span>|<span data-ttu-id="a8a4b-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="a8a4b-114">Display name</span></span>|
|<span data-ttu-id="a8a4b-115">recursos</span><span class="sxs-lookup"><span data-stu-id="a8a4b-115">resources</span></span>|<span data-ttu-id="a8a4b-116">String collection</span><span class="sxs-lookup"><span data-stu-id="a8a4b-116">String collection</span></span>|<span data-ttu-id="a8a4b-117">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="a8a4b-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8a4b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a8a4b-118">Relationships</span></span>
<span data-ttu-id="a8a4b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8a4b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a8a4b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8a4b-120">JSON Representation</span></span>
<span data-ttu-id="a8a4b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8a4b-121">Here is a JSON representation of the resource.</span></span>
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





