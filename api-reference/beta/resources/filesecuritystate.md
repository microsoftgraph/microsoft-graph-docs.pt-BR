---
title: tipo de recurso de fileSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 485addfda2707c8848c44c839f9593378943f327
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526953"
---
# <a name="filesecuritystate-resource-type"></a><span data-ttu-id="936c2-104">tipo de recurso de fileSecurityState</span><span class="sxs-lookup"><span data-stu-id="936c2-104">fileSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="936c2-105">Contém informações sobre o arquivo (não process) relacionada ao alerta.</span><span class="sxs-lookup"><span data-stu-id="936c2-105">Contains information about the file (not process) related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="936c2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="936c2-106">Properties</span></span>

| <span data-ttu-id="936c2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="936c2-107">Property</span></span>   | <span data-ttu-id="936c2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="936c2-108">Type</span></span>|<span data-ttu-id="936c2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="936c2-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="936c2-110">fileHash</span><span class="sxs-lookup"><span data-stu-id="936c2-110">fileHash</span></span>|[<span data-ttu-id="936c2-111">fileHash</span><span class="sxs-lookup"><span data-stu-id="936c2-111">fileHash</span></span>](filehash.md)|<span data-ttu-id="936c2-112">Tipo complexo contendo hashes de arquivo (criptográficos e confidenciais local).</span><span class="sxs-lookup"><span data-stu-id="936c2-112">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="936c2-113">name</span><span class="sxs-lookup"><span data-stu-id="936c2-113">name</span></span>|<span data-ttu-id="936c2-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="936c2-114">String</span></span>|<span data-ttu-id="936c2-115">Nome de arquivo (sem o caminho).</span><span class="sxs-lookup"><span data-stu-id="936c2-115">File name (without path).</span></span>|
|<span data-ttu-id="936c2-116">caminho</span><span class="sxs-lookup"><span data-stu-id="936c2-116">path</span></span>|<span data-ttu-id="936c2-117">String</span><span class="sxs-lookup"><span data-stu-id="936c2-117">String</span></span>|<span data-ttu-id="936c2-118">Caminho do arquivo completo do arquivo/imageFile.</span><span class="sxs-lookup"><span data-stu-id="936c2-118">Full file path of the file/imageFile.</span></span>|
|<span data-ttu-id="936c2-119">riskScore</span><span class="sxs-lookup"><span data-stu-id="936c2-119">riskScore</span></span>|<span data-ttu-id="936c2-120">String</span><span class="sxs-lookup"><span data-stu-id="936c2-120">String</span></span>|<span data-ttu-id="936c2-121">Provedor gerado/calculado o risco de pontuação do arquivo de alerta.</span><span class="sxs-lookup"><span data-stu-id="936c2-121">Provider generated/calculated risk score of the alert file.</span></span> <span data-ttu-id="936c2-122">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="936c2-122">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="936c2-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="936c2-123">JSON representation</span></span>

<span data-ttu-id="936c2-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="936c2-124">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "fileSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filesecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
