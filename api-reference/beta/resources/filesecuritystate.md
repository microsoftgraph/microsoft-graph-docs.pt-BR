---
title: tipo de recurso de fileSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 9d18021591b24d26577e41897111b90310746d18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869500"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="69a94-104">tipo de recurso de fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="69a94-104">fileSecurityState resource type</span></span>

 > <span data-ttu-id="69a94-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="69a94-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69a94-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="69a94-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69a94-107">Contém informações sobre o arquivo (não process) relacionada ao alerta.</span><span class="sxs-lookup"><span data-stu-id="69a94-107">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="69a94-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69a94-108">Properties</span></span>

| <span data-ttu-id="69a94-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69a94-109">Property</span></span>   | <span data-ttu-id="69a94-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="69a94-110">Type</span></span>|<span data-ttu-id="69a94-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69a94-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69a94-112">fileHash</span><span class="sxs-lookup"><span data-stu-id="69a94-112">fileHash</span></span>|[<span data-ttu-id="69a94-113">fileHash</span><span class="sxs-lookup"><span data-stu-id="69a94-113">fileHash</span></span>](filehash.md)|<span data-ttu-id="69a94-114">Tipo complexo contendo hashes de arquivo (criptográficos e confidenciais local).</span><span class="sxs-lookup"><span data-stu-id="69a94-114">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="69a94-115">name</span><span class="sxs-lookup"><span data-stu-id="69a94-115">name</span></span>|<span data-ttu-id="69a94-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69a94-116">String</span></span>|<span data-ttu-id="69a94-117">Nome de arquivo (sem o caminho).</span><span class="sxs-lookup"><span data-stu-id="69a94-117">File name (without path).</span></span>|
|<span data-ttu-id="69a94-118">caminho</span><span class="sxs-lookup"><span data-stu-id="69a94-118">path</span></span>|<span data-ttu-id="69a94-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69a94-119">String</span></span>|<span data-ttu-id="69a94-120">Caminho do arquivo completo do arquivo/imageFile.</span><span class="sxs-lookup"><span data-stu-id="69a94-120">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="69a94-121">riskScore</span><span class="sxs-lookup"><span data-stu-id="69a94-121">riskScore</span></span>|<span data-ttu-id="69a94-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="69a94-122">String</span></span>|<span data-ttu-id="69a94-123">Provedor gerado/calculado o risco de pontuação do arquivo de alerta.</span><span class="sxs-lookup"><span data-stu-id="69a94-123">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="69a94-124">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="69a94-124">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69a94-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69a94-125">JSON representation</span></span>

<span data-ttu-id="69a94-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69a94-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileSecurityState"
}-->

```json
{
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "name": "String",
  "path": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
