---
title: Tipo de recurso report
description: Descreve o recurso de relatório da API do Microsoft Graph para o Intune, que dá suporte a vários fluxos de trabalho.
localization_priority: Normal
author: rolyon
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c1a21995e763b1de27645e39badd120f86bb81fc
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866661"
---
# <a name="report-resource-type"></a><span data-ttu-id="d6078-103">Tipo de recurso report</span><span class="sxs-lookup"><span data-stu-id="d6078-103">report resource type</span></span>

<span data-ttu-id="d6078-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6078-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6078-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6078-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6078-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6078-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6078-107">Retorna o conteúdo apropriado para o contexto, incluindo:</span><span class="sxs-lookup"><span data-stu-id="d6078-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="d6078-108">Relatórios de histórico do perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6078-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="d6078-109">Relatórios de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="d6078-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="d6078-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d6078-110">Properties</span></span>
|<span data-ttu-id="d6078-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6078-111">Property</span></span>|<span data-ttu-id="d6078-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6078-112">Type</span></span>|<span data-ttu-id="d6078-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6078-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6078-114">conteúdo</span><span class="sxs-lookup"><span data-stu-id="d6078-114">content</span></span>|<span data-ttu-id="d6078-115">Fluxo</span><span class="sxs-lookup"><span data-stu-id="d6078-115">Stream</span></span>|<span data-ttu-id="d6078-116">Relatar conteúdo; os detalhes variam de acordo com o tipo de relatório.</span><span class="sxs-lookup"><span data-stu-id="d6078-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6078-117">Relações</span><span class="sxs-lookup"><span data-stu-id="d6078-117">Relationships</span></span>
<span data-ttu-id="d6078-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6078-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6078-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d6078-119">JSON Representation</span></span>
<span data-ttu-id="d6078-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d6078-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```




