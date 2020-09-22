---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75bce4536f3467452d148824e1383776bba740ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056748"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="88fff-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="88fff-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="88fff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88fff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88fff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88fff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88fff-106">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="88fff-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="88fff-107">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="88fff-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="88fff-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88fff-108">Properties</span></span>
|<span data-ttu-id="88fff-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88fff-109">Property</span></span>|<span data-ttu-id="88fff-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="88fff-110">Type</span></span>|<span data-ttu-id="88fff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="88fff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88fff-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="88fff-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="88fff-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88fff-113">String</span></span>|<span data-ttu-id="88fff-114">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="88fff-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88fff-115">Relações</span><span class="sxs-lookup"><span data-stu-id="88fff-115">Relationships</span></span>
<span data-ttu-id="88fff-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88fff-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88fff-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88fff-117">JSON Representation</span></span>
<span data-ttu-id="88fff-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88fff-118">Here is a JSON representation of the resource.</span></span>
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









