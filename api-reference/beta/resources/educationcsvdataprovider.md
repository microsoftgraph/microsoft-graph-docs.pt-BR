---
title: tipo de recurso de educationCsvDataProvider
description: 'Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.  '
author: mmast-msft
ms.openlocfilehash: 1a816d4e176147d549381465154e35cf0a821b98
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317896"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="26f57-103">tipo de recurso de educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="26f57-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="26f57-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="26f57-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="26f57-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="26f57-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="26f57-106">Usado para configurar o perfil de sincronização de dados da escola quando arquivos CSV são a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="26f57-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="26f57-107">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="26f57-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="26f57-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="26f57-108">Properties</span></span>

| <span data-ttu-id="26f57-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26f57-109">Property</span></span> | <span data-ttu-id="26f57-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="26f57-110">Type</span></span> | <span data-ttu-id="26f57-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="26f57-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="26f57-112">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="26f57-112">**customizations**</span></span> | [<span data-ttu-id="26f57-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="26f57-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="26f57-114">Personalizações opcionais a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="26f57-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="26f57-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="26f57-115">JSON representation</span></span>

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
