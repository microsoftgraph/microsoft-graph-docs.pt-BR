---
title: Tipo de recurso userRegistrationMethodSummary
description: Resumo do número de usuários registrados para cada método de autenticação.
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6ff9a079ddce0df5031eef2b1374ebb1d233d56d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132913"
---
# <a name="userregistrationmethodsummary-resource-type"></a><span data-ttu-id="b4e8d-103">Tipo de recurso userRegistrationMethodSummary</span><span class="sxs-lookup"><span data-stu-id="b4e8d-103">userRegistrationMethodSummary resource type</span></span>

<span data-ttu-id="b4e8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4e8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4e8d-105">Resumo do número de usuários registrados para cada método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-105">Summary of number of users registered for each authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="b4e8d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b4e8d-106">Methods</span></span>

| <span data-ttu-id="b4e8d-107">Método</span><span class="sxs-lookup"><span data-stu-id="b4e8d-107">Method</span></span>       | <span data-ttu-id="b4e8d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b4e8d-108">Return Type</span></span> | <span data-ttu-id="b4e8d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4e8d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b4e8d-110">usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="b4e8d-110">usersRegisteredByMethod</span></span>](../api/authenticationmethodsroot-usersregisteredbymethod.md) | <span data-ttu-id="b4e8d-111">userRegistrationMethodSummary</span><span class="sxs-lookup"><span data-stu-id="b4e8d-111">userRegistrationMethodSummary</span></span> | <span data-ttu-id="b4e8d-112">Obter o número de usuários registrados para cada método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-112">Get the number of users registered for each authentication method.</span></span> |

## <a name="properties"></a><span data-ttu-id="b4e8d-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4e8d-113">Properties</span></span>
|<span data-ttu-id="b4e8d-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4e8d-114">Property</span></span>|<span data-ttu-id="b4e8d-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4e8d-115">Type</span></span>|<span data-ttu-id="b4e8d-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4e8d-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4e8d-117">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="b4e8d-117">totalUserCount</span></span>|<span data-ttu-id="b4e8d-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b4e8d-118">Int64</span></span>|<span data-ttu-id="b4e8d-119">Número total de usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-119">Total number of users in the tenant.</span></span>|
|<span data-ttu-id="b4e8d-120">userRegistrationMethodCounts</span><span class="sxs-lookup"><span data-stu-id="b4e8d-120">userRegistrationMethodCounts</span></span>|<span data-ttu-id="b4e8d-121">[Coleção userRegistrationMethodCount](../resources/userregistrationmethodcount.md)</span><span class="sxs-lookup"><span data-stu-id="b4e8d-121">[userRegistrationMethodCount](../resources/userregistrationmethodcount.md) collection</span></span>|<span data-ttu-id="b4e8d-122">Número de usuários registrados para cada método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-122">Number of users registered for each authentication method.</span></span>|
|<span data-ttu-id="b4e8d-123">userRoles</span><span class="sxs-lookup"><span data-stu-id="b4e8d-123">userRoles</span></span>|<span data-ttu-id="b4e8d-124">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="b4e8d-124">includedUserRoles</span></span>|<span data-ttu-id="b4e8d-125">Tipo de função de usuário.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-125">User role type.</span></span> <span data-ttu-id="b4e8d-126">Os valores possíveis são: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-126">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|
|<span data-ttu-id="b4e8d-127">userTypes</span><span class="sxs-lookup"><span data-stu-id="b4e8d-127">userTypes</span></span>|<span data-ttu-id="b4e8d-128">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="b4e8d-128">includedUserTypes</span></span>|<span data-ttu-id="b4e8d-129">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-129">User type.</span></span> <span data-ttu-id="b4e8d-130">Os valores possíveis são: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-130">Possible values are: `all`, `member`, `guest`.</span></span>|

<span data-ttu-id="b4e8d-131">O valor `privilegedAdmin` consiste nas seguintes funções de administrador privilegiado:</span><span class="sxs-lookup"><span data-stu-id="b4e8d-131">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="b4e8d-132">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b4e8d-132">Global admin</span></span>
* <span data-ttu-id="b4e8d-133">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="b4e8d-133">Security admin</span></span>
* <span data-ttu-id="b4e8d-134">Administrador de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="b4e8d-134">Conditional Access admin</span></span>
* <span data-ttu-id="b4e8d-135">Administrador do Exchange</span><span class="sxs-lookup"><span data-stu-id="b4e8d-135">Exchange admin</span></span>
* <span data-ttu-id="b4e8d-136">Administrador do SharePoint</span><span class="sxs-lookup"><span data-stu-id="b4e8d-136">SharePoint admin</span></span>
* <span data-ttu-id="b4e8d-137">Administrador de help desk</span><span class="sxs-lookup"><span data-stu-id="b4e8d-137">Helpdesk admin</span></span>
* <span data-ttu-id="b4e8d-138">Administrador de faturamento</span><span class="sxs-lookup"><span data-stu-id="b4e8d-138">Billing admin</span></span>
* <span data-ttu-id="b4e8d-139">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="b4e8d-139">User admin</span></span>
* <span data-ttu-id="b4e8d-140">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="b4e8d-140">Authentication admin</span></span>

<span data-ttu-id="b4e8d-141">O valor inclui todas as funções de administrador do `admin` Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-141">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="relationships"></a><span data-ttu-id="b4e8d-142">Relações</span><span class="sxs-lookup"><span data-stu-id="b4e8d-142">Relationships</span></span>
<span data-ttu-id="b4e8d-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4e8d-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4e8d-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4e8d-144">JSON representation</span></span>
<span data-ttu-id="b4e8d-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4e8d-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationMethodCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationMethodCount"
    }
  ]
}
```
