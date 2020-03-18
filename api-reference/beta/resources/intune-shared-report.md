---
title: Tipo de recurso report
description: Descreve o recurso de relatório da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d321b5a2dadc4a459194a24224805f7443592532
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768006"
---
# <a name="report-resource-type"></a><span data-ttu-id="34fff-103">Tipo de recurso report</span><span class="sxs-lookup"><span data-stu-id="34fff-103">report resource type</span></span>

> <span data-ttu-id="34fff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34fff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34fff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34fff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34fff-106">Retorna o conteúdo apropriado para o contexto, incluindo:</span><span class="sxs-lookup"><span data-stu-id="34fff-106">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="34fff-107">Relatórios de histórico de perfil de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34fff-107">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="34fff-108">Relatórios de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="34fff-108">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="34fff-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34fff-109">Properties</span></span>
|<span data-ttu-id="34fff-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34fff-110">Property</span></span>|<span data-ttu-id="34fff-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="34fff-111">Type</span></span>|<span data-ttu-id="34fff-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="34fff-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34fff-113">conteúdo</span><span class="sxs-lookup"><span data-stu-id="34fff-113">content</span></span>|<span data-ttu-id="34fff-114">Fluxo</span><span class="sxs-lookup"><span data-stu-id="34fff-114">Stream</span></span>|<span data-ttu-id="34fff-115">Conteúdo de relatórios; os detalhes variam por tipo de relatório.</span><span class="sxs-lookup"><span data-stu-id="34fff-115">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34fff-116">Relações</span><span class="sxs-lookup"><span data-stu-id="34fff-116">Relationships</span></span>
<span data-ttu-id="34fff-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34fff-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34fff-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34fff-118">JSON Representation</span></span>
<span data-ttu-id="34fff-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34fff-119">Here is a JSON representation of the resource.</span></span>
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



