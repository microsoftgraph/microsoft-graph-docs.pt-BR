---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d48793eed6930b21defdb1f8f7aa921cdece2e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532538"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="2569a-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="2569a-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="2569a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2569a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2569a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2569a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2569a-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="2569a-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="2569a-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="2569a-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2569a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2569a-108">Properties</span></span>
|<span data-ttu-id="2569a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2569a-109">Property</span></span>|<span data-ttu-id="2569a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2569a-110">Type</span></span>|<span data-ttu-id="2569a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2569a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2569a-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="2569a-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="2569a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2569a-113">String</span></span>|<span data-ttu-id="2569a-114">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="2569a-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2569a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="2569a-115">Relationships</span></span>
<span data-ttu-id="2569a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2569a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2569a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2569a-117">JSON Representation</span></span>
<span data-ttu-id="2569a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2569a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```




