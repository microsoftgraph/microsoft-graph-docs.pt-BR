---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a6c9f18a7a02db7054f8cbc230783fb1224e5ae
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996397"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="79741-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="79741-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="79741-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79741-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79741-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79741-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79741-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="79741-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="79741-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="79741-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79741-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79741-108">Properties</span></span>
|<span data-ttu-id="79741-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79741-109">Property</span></span>|<span data-ttu-id="79741-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="79741-110">Type</span></span>|<span data-ttu-id="79741-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="79741-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79741-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="79741-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="79741-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79741-113">String</span></span>|<span data-ttu-id="79741-114">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="79741-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79741-115">Relações</span><span class="sxs-lookup"><span data-stu-id="79741-115">Relationships</span></span>
<span data-ttu-id="79741-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79741-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79741-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79741-117">JSON Representation</span></span>
<span data-ttu-id="79741-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79741-118">Here is a JSON representation of the resource.</span></span>
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





