---
title: tipo de recurso Employees
description: Um objeto Employee no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 84fccbcb9d60c97a2ce0079a9ba773a8400a8069
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504080"
---
# <a name="employees-resource-type"></a><span data-ttu-id="610ac-103">tipo de recurso Employees</span><span class="sxs-lookup"><span data-stu-id="610ac-103">employees resource type</span></span>

<span data-ttu-id="610ac-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="610ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="610ac-105">Representa um funcionário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="610ac-105">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="610ac-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="610ac-106">Methods</span></span>

| <span data-ttu-id="610ac-107">Método</span><span class="sxs-lookup"><span data-stu-id="610ac-107">Method</span></span>                                              | <span data-ttu-id="610ac-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="610ac-108">Return Type</span></span>|<span data-ttu-id="610ac-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="610ac-109">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="610ac-110">Obter funcionários</span><span class="sxs-lookup"><span data-stu-id="610ac-110">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="610ac-111">dos</span><span class="sxs-lookup"><span data-stu-id="610ac-111">employees</span></span>  |<span data-ttu-id="610ac-112">Obter um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="610ac-112">Get an employee object.</span></span>   |
|[<span data-ttu-id="610ac-113">Postar funcionários</span><span class="sxs-lookup"><span data-stu-id="610ac-113">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="610ac-114">dos</span><span class="sxs-lookup"><span data-stu-id="610ac-114">employees</span></span>  |<span data-ttu-id="610ac-115">Criar um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="610ac-115">Create an employee object.</span></span>|
|[<span data-ttu-id="610ac-116">Patch funcionários</span><span class="sxs-lookup"><span data-stu-id="610ac-116">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="610ac-117">dos</span><span class="sxs-lookup"><span data-stu-id="610ac-117">employees</span></span>  |<span data-ttu-id="610ac-118">Atualizar um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="610ac-118">Update an employee object.</span></span>|
|[<span data-ttu-id="610ac-119">Excluir funcionários</span><span class="sxs-lookup"><span data-stu-id="610ac-119">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="610ac-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="610ac-120">none</span></span>       |<span data-ttu-id="610ac-121">Excluir um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="610ac-121">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="610ac-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="610ac-122">Properties</span></span>
| <span data-ttu-id="610ac-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="610ac-123">Property</span></span>           | <span data-ttu-id="610ac-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="610ac-124">Type</span></span>   |<span data-ttu-id="610ac-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="610ac-125">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="610ac-126">id</span><span class="sxs-lookup"><span data-stu-id="610ac-126">id</span></span>                  |<span data-ttu-id="610ac-127">GUID</span><span class="sxs-lookup"><span data-stu-id="610ac-127">GUID</span></span>    |<span data-ttu-id="610ac-128">A ID do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-128">The employee ID.</span></span> <span data-ttu-id="610ac-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="610ac-129">Non-editable.</span></span>                         |
|<span data-ttu-id="610ac-130">number</span><span class="sxs-lookup"><span data-stu-id="610ac-130">number</span></span>              |<span data-ttu-id="610ac-131">string</span><span class="sxs-lookup"><span data-stu-id="610ac-131">string</span></span>  |<span data-ttu-id="610ac-132">O número do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-132">The employee number.</span></span> <span data-ttu-id="610ac-133">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="610ac-133">Read-Only.</span></span>                        |
|<span data-ttu-id="610ac-134">displayName</span><span class="sxs-lookup"><span data-stu-id="610ac-134">displayName</span></span>         |<span data-ttu-id="610ac-135">string</span><span class="sxs-lookup"><span data-stu-id="610ac-135">string</span></span>  |<span data-ttu-id="610ac-136">O funcionário de atribuído + sobrenome.</span><span class="sxs-lookup"><span data-stu-id="610ac-136">The employee givenName + surname.</span></span> <span data-ttu-id="610ac-137">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="610ac-137">Read-Only.</span></span>           |
|<span data-ttu-id="610ac-138">givenName</span><span class="sxs-lookup"><span data-stu-id="610ac-138">givenName</span></span>           |<span data-ttu-id="610ac-139">string</span><span class="sxs-lookup"><span data-stu-id="610ac-139">string</span></span>  |<span data-ttu-id="610ac-140">O nome fornecido do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-140">The given name of the employee.</span></span>                        |
|<span data-ttu-id="610ac-141">middleName</span><span class="sxs-lookup"><span data-stu-id="610ac-141">middleName</span></span>          |<span data-ttu-id="610ac-142">string</span><span class="sxs-lookup"><span data-stu-id="610ac-142">string</span></span>  |<span data-ttu-id="610ac-143">O nome do meio do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-143">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="610ac-144">surname</span><span class="sxs-lookup"><span data-stu-id="610ac-144">surname</span></span>             |<span data-ttu-id="610ac-145">string</span><span class="sxs-lookup"><span data-stu-id="610ac-145">string</span></span>  |<span data-ttu-id="610ac-146">O sobrenome do funcionário</span><span class="sxs-lookup"><span data-stu-id="610ac-146">The surname of the employee</span></span>                            |
|<span data-ttu-id="610ac-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="610ac-147">jobTitle</span></span>            |<span data-ttu-id="610ac-148">string</span><span class="sxs-lookup"><span data-stu-id="610ac-148">string</span></span>  |<span data-ttu-id="610ac-149">O nome completo do funcionário</span><span class="sxs-lookup"><span data-stu-id="610ac-149">The full name of the employee</span></span>                          |
|<span data-ttu-id="610ac-150">address</span><span class="sxs-lookup"><span data-stu-id="610ac-150">address</span></span>             |[<span data-ttu-id="610ac-151">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="610ac-151">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="610ac-152">Especifica o endereço do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-152">Specifies the employee's address.</span></span> <span data-ttu-id="610ac-153">Esse endereço aparecerá em todos os documentos de recursos do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-153">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="610ac-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="610ac-154">phoneNumber</span></span>         |<span data-ttu-id="610ac-155">string</span><span class="sxs-lookup"><span data-stu-id="610ac-155">string</span></span>  |<span data-ttu-id="610ac-156">Especifica o número de telefone do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-156">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="610ac-157">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="610ac-157">mobilePhone</span></span>         |<span data-ttu-id="610ac-158">string</span><span class="sxs-lookup"><span data-stu-id="610ac-158">string</span></span>  |<span data-ttu-id="610ac-159">Especifica o número de telefone celular do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-159">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="610ac-160">email</span><span class="sxs-lookup"><span data-stu-id="610ac-160">email</span></span>               |<span data-ttu-id="610ac-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="610ac-161">string</span></span>  |<span data-ttu-id="610ac-162">Especifica o endereço de email do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-162">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="610ac-163">personalEmail</span><span class="sxs-lookup"><span data-stu-id="610ac-163">personalEmail</span></span>       |<span data-ttu-id="610ac-164">string</span><span class="sxs-lookup"><span data-stu-id="610ac-164">string</span></span>  |<span data-ttu-id="610ac-165">Especifica o endereço de email pessoal do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-165">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="610ac-166">employmentDate</span><span class="sxs-lookup"><span data-stu-id="610ac-166">employmentDate</span></span>      |<span data-ttu-id="610ac-167">data</span><span class="sxs-lookup"><span data-stu-id="610ac-167">date</span></span>    |<span data-ttu-id="610ac-168">Especifica a data em que o funcionário começou a trabalhar para a empresa.</span><span class="sxs-lookup"><span data-stu-id="610ac-168">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="610ac-169">terminationDate</span><span class="sxs-lookup"><span data-stu-id="610ac-169">terminationDate</span></span>     |<span data-ttu-id="610ac-170">data</span><span class="sxs-lookup"><span data-stu-id="610ac-170">date</span></span>    |<span data-ttu-id="610ac-171">Especifica a data de término do funcionário, devido à aposentadoria ou à descarta, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="610ac-171">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="610ac-172">status</span><span class="sxs-lookup"><span data-stu-id="610ac-172">status</span></span>              |<span data-ttu-id="610ac-173">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="610ac-173">string</span></span>  |<span data-ttu-id="610ac-174">Especifica o status do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-174">Specifies the employee's status.</span></span> <span data-ttu-id="610ac-175">Os valores possíveis estão ativos, inativos ou terminados</span><span class="sxs-lookup"><span data-stu-id="610ac-175">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="610ac-176">birthDate</span><span class="sxs-lookup"><span data-stu-id="610ac-176">birthDate</span></span>           |<span data-ttu-id="610ac-177">data</span><span class="sxs-lookup"><span data-stu-id="610ac-177">date</span></span>    |<span data-ttu-id="610ac-178">Especifica a data de nascimento do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-178">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="610ac-179">Panorama</span><span class="sxs-lookup"><span data-stu-id="610ac-179">picture</span></span>             |<span data-ttu-id="610ac-180">stream</span><span class="sxs-lookup"><span data-stu-id="610ac-180">stream</span></span>  |<span data-ttu-id="610ac-181">A imagem do funcionário.</span><span class="sxs-lookup"><span data-stu-id="610ac-181">The employee picture.</span></span> <span data-ttu-id="610ac-182">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="610ac-182">Read-Only.</span></span>                       |
|<span data-ttu-id="610ac-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="610ac-183">lastModifiedDateTime</span></span>|<span data-ttu-id="610ac-184">datetime</span><span class="sxs-lookup"><span data-stu-id="610ac-184">datetime</span></span>|<span data-ttu-id="610ac-185">O último DateTime que o funcionário foi modificado.</span><span class="sxs-lookup"><span data-stu-id="610ac-185">The last datetime the employee was modified.</span></span> <span data-ttu-id="610ac-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="610ac-186">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="610ac-187">Relações</span><span class="sxs-lookup"><span data-stu-id="610ac-187">Relationships</span></span>
<span data-ttu-id="610ac-188">Nenhum</span><span class="sxs-lookup"><span data-stu-id="610ac-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="610ac-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="610ac-189">JSON representation</span></span>

<span data-ttu-id="610ac-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="610ac-190">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "givenName": "string",
    "middleName": "string",
    "surname": "string",
    "jobTitle": "string",
    "address": "NAV.PostalAddress",
    "phoneNumber": "string",
    "mobilePhone": "string",
    "email": "string",
    "personalEmail": "string",
    "employmentDate": "date",
    "terminationDate": "date",
    "status": "string",
    "birthDate": "date",
    "picture": "stream",
    "lastModifiedDateTime": "datetime"
}

```

