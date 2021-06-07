---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc0f0f7175a5b2cfb6be8f2b09b83ad263ae6050
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758859"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="3c60f-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="3c60f-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="3c60f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c60f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c60f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c60f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c60f-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="3c60f-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="3c60f-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="3c60f-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3c60f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c60f-108">Properties</span></span>
|<span data-ttu-id="3c60f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c60f-109">Property</span></span>|<span data-ttu-id="3c60f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c60f-110">Type</span></span>|<span data-ttu-id="3c60f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c60f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c60f-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="3c60f-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="3c60f-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c60f-113">String</span></span>|<span data-ttu-id="3c60f-114">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="3c60f-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c60f-115">Relações</span><span class="sxs-lookup"><span data-stu-id="3c60f-115">Relationships</span></span>
<span data-ttu-id="3c60f-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c60f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c60f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c60f-117">JSON Representation</span></span>
<span data-ttu-id="3c60f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c60f-118">Here is a JSON representation of the resource.</span></span>
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




