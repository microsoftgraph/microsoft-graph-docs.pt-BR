---
title: tipo de recurso groupPolicyUploadedLanguageFile
description: A entidade representa um arquivo XML de ADML (idioma de modelo administrativo) carregado pelo administrador.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c3b2a4fd4ab035dd072af8db0cd6897bfd7d9153
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43385899"
---
# <a name="grouppolicyuploadedlanguagefile-resource-type"></a><span data-ttu-id="010dd-103">tipo de recurso groupPolicyUploadedLanguageFile</span><span class="sxs-lookup"><span data-stu-id="010dd-103">groupPolicyUploadedLanguageFile resource type</span></span>

<span data-ttu-id="010dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="010dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="010dd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="010dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="010dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="010dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="010dd-107">A entidade representa um arquivo XML de ADML (idioma de modelo administrativo) carregado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="010dd-107">The entity represents an ADML (Administrative Template language) XML file uploaded by Administrator.</span></span>

## <a name="properties"></a><span data-ttu-id="010dd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="010dd-108">Properties</span></span>
|<span data-ttu-id="010dd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="010dd-109">Property</span></span>|<span data-ttu-id="010dd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="010dd-110">Type</span></span>|<span data-ttu-id="010dd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="010dd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="010dd-112">fileName</span><span class="sxs-lookup"><span data-stu-id="010dd-112">fileName</span></span>|<span data-ttu-id="010dd-113">String</span><span class="sxs-lookup"><span data-stu-id="010dd-113">String</span></span>|<span data-ttu-id="010dd-114">O nome de arquivo do arquivo ADML carregado.</span><span class="sxs-lookup"><span data-stu-id="010dd-114">The file name of the uploaded ADML file.</span></span>|
|<span data-ttu-id="010dd-115">Campo</span><span class="sxs-lookup"><span data-stu-id="010dd-115">languageCode</span></span>|<span data-ttu-id="010dd-116">String</span><span class="sxs-lookup"><span data-stu-id="010dd-116">String</span></span>|<span data-ttu-id="010dd-117">O código de idioma do arquivo ADML carregado.</span><span class="sxs-lookup"><span data-stu-id="010dd-117">The language code of the uploaded ADML file.</span></span>|
|<span data-ttu-id="010dd-118">conteúdo</span><span class="sxs-lookup"><span data-stu-id="010dd-118">content</span></span>|<span data-ttu-id="010dd-119">Binária</span><span class="sxs-lookup"><span data-stu-id="010dd-119">Binary</span></span>|<span data-ttu-id="010dd-120">O conteúdo do arquivo ADML carregado.</span><span class="sxs-lookup"><span data-stu-id="010dd-120">The contents of the uploaded ADML file.</span></span>|
|<span data-ttu-id="010dd-121">id</span><span class="sxs-lookup"><span data-stu-id="010dd-121">id</span></span>|<span data-ttu-id="010dd-122">String</span><span class="sxs-lookup"><span data-stu-id="010dd-122">String</span></span>|<span data-ttu-id="010dd-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="010dd-123">Key of the entity.</span></span>|
|<span data-ttu-id="010dd-124">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="010dd-124">lastModifiedDateTime</span></span>|<span data-ttu-id="010dd-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="010dd-125">DateTimeOffset</span></span>|<span data-ttu-id="010dd-126">A data e a hora em que a entidade foi modificada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="010dd-126">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="010dd-127">Relações</span><span class="sxs-lookup"><span data-stu-id="010dd-127">Relationships</span></span>
<span data-ttu-id="010dd-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="010dd-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="010dd-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="010dd-129">JSON Representation</span></span>
<span data-ttu-id="010dd-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="010dd-130">Here is a JSON representation of the resource.</span></span>
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



