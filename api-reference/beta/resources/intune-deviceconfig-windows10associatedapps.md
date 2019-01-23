---
title: tipo de recurso de windows10AssociatedApps
description: Definição de aplicativo do Windows 10 associados.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5dd5b664bde2970caa4b09c027592684b9ecd5e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425915"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="98821-103">tipo de recurso de windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="98821-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="98821-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="98821-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="98821-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="98821-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98821-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="98821-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98821-107">Definição de aplicativo do Windows 10 associados.</span><span class="sxs-lookup"><span data-stu-id="98821-107">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="98821-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98821-108">Properties</span></span>
|<span data-ttu-id="98821-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98821-109">Property</span></span>|<span data-ttu-id="98821-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="98821-110">Type</span></span>|<span data-ttu-id="98821-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="98821-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98821-112">tipo de aplicativo</span><span class="sxs-lookup"><span data-stu-id="98821-112">appType</span></span>|[<span data-ttu-id="98821-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="98821-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="98821-114">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="98821-114">Application type.</span></span> <span data-ttu-id="98821-115">Os valores possíveis são: `desktop` e `universal`.</span><span class="sxs-lookup"><span data-stu-id="98821-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="98821-116">identificador</span><span class="sxs-lookup"><span data-stu-id="98821-116">identifier</span></span>|<span data-ttu-id="98821-117">String</span><span class="sxs-lookup"><span data-stu-id="98821-117">String</span></span>|<span data-ttu-id="98821-118">Identificador.</span><span class="sxs-lookup"><span data-stu-id="98821-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98821-119">Relações</span><span class="sxs-lookup"><span data-stu-id="98821-119">Relationships</span></span>
<span data-ttu-id="98821-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98821-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98821-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98821-121">JSON Representation</span></span>
<span data-ttu-id="98821-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98821-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```




