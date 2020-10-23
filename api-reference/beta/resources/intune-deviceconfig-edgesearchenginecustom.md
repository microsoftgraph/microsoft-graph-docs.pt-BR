---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 85e25641fe03a4baa090a3d1fa7afe33978a9c35
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728588"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="676f5-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="676f5-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="676f5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="676f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="676f5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="676f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="676f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="676f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="676f5-107">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="676f5-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="676f5-108">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="676f5-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="676f5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="676f5-109">Properties</span></span>
|<span data-ttu-id="676f5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="676f5-110">Property</span></span>|<span data-ttu-id="676f5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="676f5-111">Type</span></span>|<span data-ttu-id="676f5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="676f5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="676f5-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="676f5-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="676f5-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="676f5-114">String</span></span>|<span data-ttu-id="676f5-115">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="676f5-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="676f5-116">Relações</span><span class="sxs-lookup"><span data-stu-id="676f5-116">Relationships</span></span>
<span data-ttu-id="676f5-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="676f5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="676f5-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="676f5-118">JSON Representation</span></span>
<span data-ttu-id="676f5-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="676f5-119">Here is a JSON representation of the resource.</span></span>
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





