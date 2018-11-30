---
title: tipo de recurso de educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.  '
ms.openlocfilehash: a3079b4f18c74c95fb0f8646116f2c7901d17b3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033528"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="4d7f0-103">tipo de recurso de educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="4d7f0-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="4d7f0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4d7f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4d7f0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4d7f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4d7f0-106">Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="4d7f0-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="4d7f0-107">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="4d7f0-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4d7f0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d7f0-108">Properties</span></span>

| <span data-ttu-id="4d7f0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d7f0-109">Property</span></span> | <span data-ttu-id="4d7f0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d7f0-110">Type</span></span> | <span data-ttu-id="4d7f0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d7f0-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4d7f0-112">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="4d7f0-112">**customizations**</span></span> | [<span data-ttu-id="4d7f0-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="4d7f0-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="4d7f0-114">Personalizações opcionais a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4d7f0-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d7f0-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d7f0-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
