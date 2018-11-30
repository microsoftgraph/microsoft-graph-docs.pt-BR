---
title: tipo de recurso de educationFileSynchronizationVerificationMessage
description: Representa um erro retornado ao cliente em resposta a uma solicitação para iniciar a sincronização de perfis de dados baseada em CSV escola. O recurso irá conter erros resultantes da verificação. Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).
ms.openlocfilehash: cf685e0619c5600340df68ba86ecaef11a8a435d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033525"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a><span data-ttu-id="13faf-105">tipo de recurso de educationFileSynchronizationVerificationMessage</span><span class="sxs-lookup"><span data-stu-id="13faf-105">educationFileSynchronizationVerificationMessage resource type</span></span>

> <span data-ttu-id="13faf-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="13faf-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13faf-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="13faf-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="13faf-108">Representa um erro retornado ao cliente em resposta a uma solicitação para [Iniciar a sincronização](../api/educationsynchronizationprofile-start.md) de perfis de dados baseada em CSV escola.</span><span class="sxs-lookup"><span data-stu-id="13faf-108">Represents an error returned to the client in response to a request to [start synchronization](../api/educationsynchronizationprofile-start.md) for CSV-based school data profiles.</span></span> <span data-ttu-id="13faf-109">O recurso irá conter erros resultantes da verificação.</span><span class="sxs-lookup"><span data-stu-id="13faf-109">The resource will contain errors that result from the verification.</span></span> <span data-ttu-id="13faf-110">Os usuários devem corrigir os dados de origem antes de reiniciar a solicitação para sincronizar com o Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="13faf-110">Users must fix the source data before you restart the request to synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="13faf-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13faf-111">Properties</span></span>

| <span data-ttu-id="13faf-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13faf-112">Property</span></span> | <span data-ttu-id="13faf-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="13faf-113">Type</span></span> | <span data-ttu-id="13faf-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="13faf-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="13faf-115">**type**</span><span class="sxs-lookup"><span data-stu-id="13faf-115">**type**</span></span> | <span data-ttu-id="13faf-116">string</span><span class="sxs-lookup"><span data-stu-id="13faf-116">string</span></span> | <span data-ttu-id="13faf-117">Tipo da mensagem.</span><span class="sxs-lookup"><span data-stu-id="13faf-117">Type of the message.</span></span> <span data-ttu-id="13faf-118">Os valores possíveis são: `error`, `warning`, `information`.</span><span class="sxs-lookup"><span data-stu-id="13faf-118">Possible values are: `error`, `warning`, `information`.</span></span> | 
| <span data-ttu-id="13faf-119">**FileName**</span><span class="sxs-lookup"><span data-stu-id="13faf-119">**filename**</span></span> | <span data-ttu-id="13faf-120">string</span><span class="sxs-lookup"><span data-stu-id="13faf-120">string</span></span> | <span data-ttu-id="13faf-121">Arquivo de origem que contém o erro.</span><span class="sxs-lookup"><span data-stu-id="13faf-121">Source file that contains the error.</span></span> |
| <span data-ttu-id="13faf-122">**description**</span><span class="sxs-lookup"><span data-stu-id="13faf-122">**description**</span></span> | <span data-ttu-id="13faf-123">string</span><span class="sxs-lookup"><span data-stu-id="13faf-123">string</span></span> | <span data-ttu-id="13faf-124">Informações detalhadas sobre o tipo de mensagem.</span><span class="sxs-lookup"><span data-stu-id="13faf-124">Detailed information about the message type.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="13faf-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13faf-125">JSON representation</span></span>

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