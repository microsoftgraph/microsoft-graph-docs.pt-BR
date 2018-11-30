---
title: tipo de recurso de governancePermission
description: 'Representa a permissão de acesso que tenha um governanceSubject um governanceResource específico.  '
ms.openlocfilehash: d7b3e1eb70c89c278ccc2a8b3e9a16e265e4ae97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037736"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="22fa7-103">tipo de recurso de governancePermission</span><span class="sxs-lookup"><span data-stu-id="22fa7-103">governancePermission resource type</span></span>

> <span data-ttu-id="22fa7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="22fa7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22fa7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22fa7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22fa7-106">Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem um específicos [governanceResource](../resources/governanceresource.md).</span><span class="sxs-lookup"><span data-stu-id="22fa7-106">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="22fa7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22fa7-107">Properties</span></span>
| <span data-ttu-id="22fa7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22fa7-108">Property</span></span>     | <span data-ttu-id="22fa7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="22fa7-109">Type</span></span>   |<span data-ttu-id="22fa7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="22fa7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22fa7-111">accessLevel</span><span class="sxs-lookup"><span data-stu-id="22fa7-111">accessLevel</span></span>|<span data-ttu-id="22fa7-112">String</span><span class="sxs-lookup"><span data-stu-id="22fa7-112">String</span></span>|<span data-ttu-id="22fa7-113">O nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="22fa7-113">The access level.</span></span> <span data-ttu-id="22fa7-114">Valores válidos: ``None``, ``UserRead``, ``AdminRead``, e ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="22fa7-114">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="22fa7-115">isActive</span><span class="sxs-lookup"><span data-stu-id="22fa7-115">isActive</span></span>|<span data-ttu-id="22fa7-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="22fa7-116">Boolean</span></span>|<span data-ttu-id="22fa7-117">Indique se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="22fa7-117">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="22fa7-118">isEligible</span><span class="sxs-lookup"><span data-stu-id="22fa7-118">isEligible</span></span>|<span data-ttu-id="22fa7-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="22fa7-119">Boolean</span></span>|<span data-ttu-id="22fa7-120">Indica se o solicitante tem qualquer atribuição de função elegíveis para o nível de acesso.</span><span class="sxs-lookup"><span data-stu-id="22fa7-120">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22fa7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22fa7-121">JSON representation</span></span>

<span data-ttu-id="22fa7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22fa7-122">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```