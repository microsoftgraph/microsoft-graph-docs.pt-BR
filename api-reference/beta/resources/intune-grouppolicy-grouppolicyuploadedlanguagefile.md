---
title: tipo de recurso groupPolicyUploadedLanguageFile
description: A entidade representa um arquivo XML de ADML (idioma de modelo administrativo) carregado pelo administrador.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc70d0ff85cebc567b9efc67b87bb57e2e8337fa
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707686"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a><span data-ttu-id="9932d-103">tipo de recurso groupPolicyUploadedLanguageFile</span><span class="sxs-lookup"><span data-stu-id="9932d-103">groupPolicyUploadedLanguageFile resource type</span></span>

<span data-ttu-id="9932d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9932d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9932d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9932d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9932d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9932d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9932d-107">A entidade representa um arquivo XML de ADML (idioma de modelo administrativo) carregado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9932d-107">The entity represents an ADML (Administrative Template language) XML file uploaded by Administrator.</span></span>

## <a name="properties"></a><span data-ttu-id="9932d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9932d-108">Properties</span></span>
|<span data-ttu-id="9932d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9932d-109">Property</span></span>|<span data-ttu-id="9932d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9932d-110">Type</span></span>|<span data-ttu-id="9932d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9932d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9932d-112">fileName</span><span class="sxs-lookup"><span data-stu-id="9932d-112">fileName</span></span>|<span data-ttu-id="9932d-113">String</span><span class="sxs-lookup"><span data-stu-id="9932d-113">String</span></span>|<span data-ttu-id="9932d-114">O nome de arquivo do arquivo ADML carregado.</span><span class="sxs-lookup"><span data-stu-id="9932d-114">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="9932d-115">Campo</span><span class="sxs-lookup"><span data-stu-id="9932d-115">languageCode</span></span>|<span data-ttu-id="9932d-116">String</span><span class="sxs-lookup"><span data-stu-id="9932d-116">String</span></span>|<span data-ttu-id="9932d-117">O código de idioma do arquivo ADML carregado.</span><span class="sxs-lookup"><span data-stu-id="9932d-117">The language code of the uploaded ADML file.</span></span>|
|<span data-ttu-id="9932d-118">conteúdo</span><span class="sxs-lookup"><span data-stu-id="9932d-118">content</span></span>|<span data-ttu-id="9932d-119">Binária</span><span class="sxs-lookup"><span data-stu-id="9932d-119">Binary</span></span>|<span data-ttu-id="9932d-120">O conteúdo do arquivo ADML carregado.</span><span class="sxs-lookup"><span data-stu-id="9932d-120">The contents of the uploaded ADML file.</span></span>|
|<span data-ttu-id="9932d-121">id</span><span class="sxs-lookup"><span data-stu-id="9932d-121">id</span></span>|<span data-ttu-id="9932d-122">String</span><span class="sxs-lookup"><span data-stu-id="9932d-122">String</span></span>|<span data-ttu-id="9932d-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9932d-123">Key of the entity.</span></span>|
|<span data-ttu-id="9932d-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9932d-124">lastModifiedDateTime</span></span>|<span data-ttu-id="9932d-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9932d-125">DateTimeOffset</span></span>|<span data-ttu-id="9932d-126">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9932d-126">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9932d-127">Relações</span><span class="sxs-lookup"><span data-stu-id="9932d-127">Relationships</span></span>
<span data-ttu-id="9932d-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9932d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9932d-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9932d-129">JSON Representation</span></span>
<span data-ttu-id="9932d-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9932d-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedLanguageFile",
  "fileName": "String",
  "languageCode": "String",
  "content": "binary",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





