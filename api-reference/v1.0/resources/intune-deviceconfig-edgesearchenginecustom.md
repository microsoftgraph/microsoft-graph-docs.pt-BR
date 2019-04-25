---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 523a2de33619886997cbcb052079bbf2937c9d48
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541224"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="fbfc5-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="fbfc5-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="fbfc5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbfc5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbfc5-105">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="fbfc5-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="fbfc5-106">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="fbfc5-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbfc5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbfc5-107">Properties</span></span>
|<span data-ttu-id="fbfc5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbfc5-108">Property</span></span>|<span data-ttu-id="fbfc5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbfc5-109">Type</span></span>|<span data-ttu-id="fbfc5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbfc5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbfc5-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="fbfc5-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="fbfc5-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbfc5-112">String</span></span>|<span data-ttu-id="fbfc5-113">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fbfc5-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbfc5-114">Relações</span><span class="sxs-lookup"><span data-stu-id="fbfc5-114">Relationships</span></span>
<span data-ttu-id="fbfc5-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbfc5-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbfc5-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbfc5-116">JSON Representation</span></span>
<span data-ttu-id="fbfc5-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbfc5-117">Here is a JSON representation of the resource.</span></span>
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



