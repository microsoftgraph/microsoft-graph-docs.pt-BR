---
title: Tipo de recurso userRegistrationFeatureSummary
description: Resumo de usuários capazes de autenticação multifa factor, redefinição Self-Service senha e autenticação sem senha.
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 291da483380d6e1d65b5db527128098b8b416c83
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132927"
---
# <a name="userregistrationfeaturesummary-resource-type"></a><span data-ttu-id="b0c93-103">Tipo de recurso userRegistrationFeatureSummary</span><span class="sxs-lookup"><span data-stu-id="b0c93-103">userRegistrationFeatureSummary resource type</span></span>

<span data-ttu-id="b0c93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0c93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0c93-105">Representa o estado atual de quantos usuários em sua organização são capazes de autenticação multifafa, redefinição de senha de autoatendado e autenticação sem senha.</span><span class="sxs-lookup"><span data-stu-id="b0c93-105">Represents the current state of how many users in your organization are capable of multi-factor authentication, self-service password reset and passwordless authentication.</span></span>

## <a name="methods"></a><span data-ttu-id="b0c93-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b0c93-106">Methods</span></span>

| <span data-ttu-id="b0c93-107">Método</span><span class="sxs-lookup"><span data-stu-id="b0c93-107">Method</span></span>       | <span data-ttu-id="b0c93-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b0c93-108">Return Type</span></span> | <span data-ttu-id="b0c93-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c93-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b0c93-110">usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="b0c93-110">usersRegisteredByFeature</span></span>](../api/authenticationmethodsroot-usersregisteredbyfeature.md) | <span data-ttu-id="b0c93-111">userRegistrationFeatureSummary</span><span class="sxs-lookup"><span data-stu-id="b0c93-111">userRegistrationFeatureSummary</span></span> | <span data-ttu-id="b0c93-112">Obter o número de usuários capazes de autenticação multifa factor, Self-Service redefinição de senha e autenticação sem senha.</span><span class="sxs-lookup"><span data-stu-id="b0c93-112">Get the number of users capable of Multi-Factor Authentication, Self-Service Password Reset, and Passwordless authentication.</span></span> |

## <a name="properties"></a><span data-ttu-id="b0c93-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0c93-113">Properties</span></span>
|<span data-ttu-id="b0c93-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0c93-114">Property</span></span>|<span data-ttu-id="b0c93-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0c93-115">Type</span></span>|<span data-ttu-id="b0c93-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0c93-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0c93-117">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="b0c93-117">totalUserCount</span></span>|<span data-ttu-id="b0c93-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b0c93-118">Int64</span></span>|<span data-ttu-id="b0c93-119">Número total de contas de usuários, excluindo aquelas bloqueadas</span><span class="sxs-lookup"><span data-stu-id="b0c93-119">Total number of users accounts, excluding those that are blocked</span></span>|
|<span data-ttu-id="b0c93-120">userRegistrationFeatureCounts</span><span class="sxs-lookup"><span data-stu-id="b0c93-120">userRegistrationFeatureCounts</span></span>|<span data-ttu-id="b0c93-121">[Coleção userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md)</span><span class="sxs-lookup"><span data-stu-id="b0c93-121">[userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md) collection</span></span>|<span data-ttu-id="b0c93-122">Número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha.</span><span class="sxs-lookup"><span data-stu-id="b0c93-122">Number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span>|
|<span data-ttu-id="b0c93-123">userRoles</span><span class="sxs-lookup"><span data-stu-id="b0c93-123">userRoles</span></span>|<span data-ttu-id="b0c93-124">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="b0c93-124">includedUserRoles</span></span>|<span data-ttu-id="b0c93-125">Tipo de função de usuário.</span><span class="sxs-lookup"><span data-stu-id="b0c93-125">User role type.</span></span> <span data-ttu-id="b0c93-126">Os valores possíveis são: `all`, `privilegedAdmin`, `admin`, `user`.</span><span class="sxs-lookup"><span data-stu-id="b0c93-126">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|
|<span data-ttu-id="b0c93-127">userTypes</span><span class="sxs-lookup"><span data-stu-id="b0c93-127">userTypes</span></span>|<span data-ttu-id="b0c93-128">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="b0c93-128">includedUserTypes</span></span>|<span data-ttu-id="b0c93-129">Tipo de usuário.</span><span class="sxs-lookup"><span data-stu-id="b0c93-129">User type.</span></span> <span data-ttu-id="b0c93-130">Os valores possíveis são: `all`, `member`, `guest`.</span><span class="sxs-lookup"><span data-stu-id="b0c93-130">Possible values are: `all`, `member`, `guest`.</span></span>|

<span data-ttu-id="b0c93-131">O valor `privilegedAdmin` consiste nas seguintes funções de administrador privilegiado:</span><span class="sxs-lookup"><span data-stu-id="b0c93-131">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="b0c93-132">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b0c93-132">Global admin</span></span>
* <span data-ttu-id="b0c93-133">Administrador de segurança</span><span class="sxs-lookup"><span data-stu-id="b0c93-133">Security admin</span></span>
* <span data-ttu-id="b0c93-134">Administrador de acesso condicional</span><span class="sxs-lookup"><span data-stu-id="b0c93-134">Conditional Access admin</span></span>
* <span data-ttu-id="b0c93-135">Administrador do Exchange</span><span class="sxs-lookup"><span data-stu-id="b0c93-135">Exchange admin</span></span>
* <span data-ttu-id="b0c93-136">Administrador do SharePoint</span><span class="sxs-lookup"><span data-stu-id="b0c93-136">SharePoint admin</span></span>
* <span data-ttu-id="b0c93-137">Administrador de help desk</span><span class="sxs-lookup"><span data-stu-id="b0c93-137">Helpdesk admin</span></span>
* <span data-ttu-id="b0c93-138">Administrador de faturamento</span><span class="sxs-lookup"><span data-stu-id="b0c93-138">Billing admin</span></span>
* <span data-ttu-id="b0c93-139">Administrador de usuários</span><span class="sxs-lookup"><span data-stu-id="b0c93-139">User admin</span></span>
* <span data-ttu-id="b0c93-140">Administrador de autenticação</span><span class="sxs-lookup"><span data-stu-id="b0c93-140">Authentication admin</span></span>

<span data-ttu-id="b0c93-141">O valor inclui todas as funções de administrador do `admin` Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0c93-141">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="relationships"></a><span data-ttu-id="b0c93-142">Relações</span><span class="sxs-lookup"><span data-stu-id="b0c93-142">Relationships</span></span>
<span data-ttu-id="b0c93-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0c93-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0c93-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0c93-144">JSON representation</span></span>
<span data-ttu-id="b0c93-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0c93-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationFeatureCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
    }
  ]
}
```
