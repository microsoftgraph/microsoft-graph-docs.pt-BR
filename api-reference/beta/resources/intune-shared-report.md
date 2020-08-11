---
title: Tipo de recurso report
description: Descreve o recurso de relatório da API do Microsoft Graph para o Intune, que oferece suporte a vários fluxos de trabalho.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f017ce3ec744bb86ee3ea6e9820a0e29f8505514
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630218"
---
# <a name="report-resource-type"></a><span data-ttu-id="14cfc-103">Tipo de recurso report</span><span class="sxs-lookup"><span data-stu-id="14cfc-103">report resource type</span></span>

<span data-ttu-id="14cfc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14cfc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="14cfc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14cfc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14cfc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14cfc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14cfc-107">Retorna o conteúdo apropriado para o contexto, incluindo:</span><span class="sxs-lookup"><span data-stu-id="14cfc-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="14cfc-108">Relatórios de histórico de perfil de configuração de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="14cfc-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="14cfc-109">Relatórios de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="14cfc-109">Enrollment failure reports.</span></span>
- <span data-ttu-id="14cfc-110">Relatórios de uso do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="14cfc-110">Microsoft 365 usage reports</span></span>

## <a name="properties"></a><span data-ttu-id="14cfc-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="14cfc-111">Properties</span></span>
|<span data-ttu-id="14cfc-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14cfc-112">Property</span></span>|<span data-ttu-id="14cfc-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="14cfc-113">Type</span></span>|<span data-ttu-id="14cfc-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="14cfc-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14cfc-115">conteúdo</span><span class="sxs-lookup"><span data-stu-id="14cfc-115">content</span></span>|<span data-ttu-id="14cfc-116">Fluxo</span><span class="sxs-lookup"><span data-stu-id="14cfc-116">Stream</span></span>|<span data-ttu-id="14cfc-117">Conteúdo de relatórios; os detalhes variam por tipo de relatório.</span><span class="sxs-lookup"><span data-stu-id="14cfc-117">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14cfc-118">Relações</span><span class="sxs-lookup"><span data-stu-id="14cfc-118">Relationships</span></span>
<span data-ttu-id="14cfc-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="14cfc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14cfc-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="14cfc-120">JSON Representation</span></span>
<span data-ttu-id="14cfc-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="14cfc-121">Here is a JSON representation of the resource.</span></span>
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



