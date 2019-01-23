---
title: Tipo de recurso edgeSearchEngineCustom
description: Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 69395d09c01c1b92f2ae3ee1abf26eeff09618f8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425978"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="fbb91-103">Tipo de recurso edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="fbb91-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="fbb91-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbb91-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fbb91-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbb91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbb91-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fbb91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbb91-107">Permite que os administradores de TI configurem um mecanismo de pesquisa padrão personalizado para dispositivos controlados por MDM.</span><span class="sxs-lookup"><span data-stu-id="fbb91-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="fbb91-108">Herda de [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="fbb91-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbb91-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbb91-109">Properties</span></span>
|<span data-ttu-id="fbb91-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbb91-110">Property</span></span>|<span data-ttu-id="fbb91-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbb91-111">Type</span></span>|<span data-ttu-id="fbb91-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbb91-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbb91-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="fbb91-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="fbb91-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbb91-114">String</span></span>|<span data-ttu-id="fbb91-115">Aponta para um link https que contém o arquivo xml de OpenSearch que contém no mínimo o nome curto e a URL do mecanismo de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="fbb91-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbb91-116">Relações</span><span class="sxs-lookup"><span data-stu-id="fbb91-116">Relationships</span></span>
<span data-ttu-id="fbb91-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbb91-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbb91-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbb91-118">JSON Representation</span></span>
<span data-ttu-id="fbb91-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbb91-119">Here is a JSON representation of the resource.</span></span>
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




