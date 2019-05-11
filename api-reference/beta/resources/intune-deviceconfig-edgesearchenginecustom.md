---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de856edf13a8d97e54925ca42537e977351675d7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946704"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="c93d8-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="c93d8-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="c93d8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c93d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c93d8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c93d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c93d8-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="c93d8-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="c93d8-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="c93d8-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c93d8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c93d8-108">Properties</span></span>
|<span data-ttu-id="c93d8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c93d8-109">Property</span></span>|<span data-ttu-id="c93d8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c93d8-110">Type</span></span>|<span data-ttu-id="c93d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c93d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c93d8-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="c93d8-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="c93d8-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c93d8-113">String</span></span>|<span data-ttu-id="c93d8-114">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c93d8-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c93d8-115">Relações</span><span class="sxs-lookup"><span data-stu-id="c93d8-115">Relationships</span></span>
<span data-ttu-id="c93d8-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c93d8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c93d8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c93d8-117">JSON Representation</span></span>
<span data-ttu-id="c93d8-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c93d8-118">Here is a JSON representation of the resource.</span></span>
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




