---
title: tipo de recurso de educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados baseada em CSV escola. O recurso irá conter erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).
author: mmast-msft
ms.openlocfilehash: f2826f779aac3ba41146b6677f3d1e0364be92a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336061"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="b312d-105">tipo de recurso de educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="b312d-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="b312d-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b312d-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b312d-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b312d-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b312d-108">Representa um erro retornado ao cliente em resposta a uma solicitação para [Iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados baseada em CSV escola.</span><span class="sxs-lookup"><span data-stu-id="b312d-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="b312d-109">O recurso irá conter erros resultantes da verificação.</span><span class="sxs-lookup"><span data-stu-id="b312d-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="b312d-110">Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="b312d-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="b312d-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b312d-111">Properties</span></span>

| <span data-ttu-id="b312d-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b312d-112">Property</span></span> | <span data-ttu-id="b312d-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b312d-113">Type</span></span> | <span data-ttu-id="b312d-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b312d-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b312d-115">**type**</span><span class="sxs-lookup"><span data-stu-id="b312d-115">**type**</span></span> | <span data-ttu-id="b312d-116">string</span><span class="sxs-lookup"><span data-stu-id="b312d-116">string</span></span> | <span data-ttu-id="b312d-117">Tipo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="b312d-117">Type of the message.</span></span> <span data-ttu-id="b312d-118">Os valores possíveis são: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="b312d-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="b312d-119">**FileName**</span><span class="sxs-lookup"><span data-stu-id="b312d-119">**filename**</span></span> | <span data-ttu-id="b312d-120">string</span><span class="sxs-lookup"><span data-stu-id="b312d-120">string</span></span> | <span data-ttu-id="b312d-121">Arquivo de origem que contém o erro.</span><span class="sxs-lookup"><span data-stu-id="b312d-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="b312d-122">**description**</span><span class="sxs-lookup"><span data-stu-id="b312d-122">**description**</span></span> | <span data-ttu-id="b312d-123">string</span><span class="sxs-lookup"><span data-stu-id="b312d-123">string</span></span> | <span data-ttu-id="b312d-124">Informações detalhadas sobre o tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="b312d-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b312d-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b312d-125">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```