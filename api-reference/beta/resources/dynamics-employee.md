---
title: tipo de recurso Employees
description: Um objeto Employee no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: d404a1ede257f3a31371dba31c37ff329452fccd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071336"
---
# <a name="employees-resource-type"></a><span data-ttu-id="b3e01-103">tipo de recurso Employees</span><span class="sxs-lookup"><span data-stu-id="b3e01-103">employees resource type</span></span>

<span data-ttu-id="b3e01-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3e01-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3e01-105">Representa um funcionário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="b3e01-105">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="b3e01-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b3e01-106">Methods</span></span>

| <span data-ttu-id="b3e01-107">Método</span><span class="sxs-lookup"><span data-stu-id="b3e01-107">Method</span></span>                                              | <span data-ttu-id="b3e01-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b3e01-108">Return Type</span></span>|<span data-ttu-id="b3e01-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3e01-109">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="b3e01-110">Obter funcionários</span><span class="sxs-lookup"><span data-stu-id="b3e01-110">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="b3e01-111">dos</span><span class="sxs-lookup"><span data-stu-id="b3e01-111">employees</span></span>  |<span data-ttu-id="b3e01-112">Obter um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="b3e01-112">Get an employee object.</span></span>   |
|[<span data-ttu-id="b3e01-113">Postar funcionários</span><span class="sxs-lookup"><span data-stu-id="b3e01-113">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="b3e01-114">dos</span><span class="sxs-lookup"><span data-stu-id="b3e01-114">employees</span></span>  |<span data-ttu-id="b3e01-115">Criar um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="b3e01-115">Create an employee object.</span></span>|
|[<span data-ttu-id="b3e01-116">Patch funcionários</span><span class="sxs-lookup"><span data-stu-id="b3e01-116">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="b3e01-117">dos</span><span class="sxs-lookup"><span data-stu-id="b3e01-117">employees</span></span>  |<span data-ttu-id="b3e01-118">Atualizar um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="b3e01-118">Update an employee object.</span></span>|
|[<span data-ttu-id="b3e01-119">Excluir funcionários</span><span class="sxs-lookup"><span data-stu-id="b3e01-119">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="b3e01-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b3e01-120">none</span></span>       |<span data-ttu-id="b3e01-121">Excluir um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="b3e01-121">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3e01-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b3e01-122">Properties</span></span>
| <span data-ttu-id="b3e01-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b3e01-123">Property</span></span>           | <span data-ttu-id="b3e01-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="b3e01-124">Type</span></span>   |<span data-ttu-id="b3e01-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3e01-125">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="b3e01-126">id</span><span class="sxs-lookup"><span data-stu-id="b3e01-126">id</span></span>                  |<span data-ttu-id="b3e01-127">GUID</span><span class="sxs-lookup"><span data-stu-id="b3e01-127">GUID</span></span>    |<span data-ttu-id="b3e01-128">A ID do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-128">The employee ID.</span></span> <span data-ttu-id="b3e01-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="b3e01-129">Non-editable.</span></span>                         |
|<span data-ttu-id="b3e01-130">number</span><span class="sxs-lookup"><span data-stu-id="b3e01-130">number</span></span>              |<span data-ttu-id="b3e01-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-131">string</span></span>  |<span data-ttu-id="b3e01-132">O número do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-132">The employee number.</span></span> <span data-ttu-id="b3e01-133">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b3e01-133">Read-Only.</span></span>                        |
|<span data-ttu-id="b3e01-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b3e01-134">displayName</span></span>         |<span data-ttu-id="b3e01-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-135">string</span></span>  |<span data-ttu-id="b3e01-136">O funcionário de atribuído + sobrenome.</span><span class="sxs-lookup"><span data-stu-id="b3e01-136">The employee givenName + surname.</span></span> <span data-ttu-id="b3e01-137">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b3e01-137">Read-Only.</span></span>           |
|<span data-ttu-id="b3e01-138">givenName</span><span class="sxs-lookup"><span data-stu-id="b3e01-138">givenName</span></span>           |<span data-ttu-id="b3e01-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-139">string</span></span>  |<span data-ttu-id="b3e01-140">O nome fornecido do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-140">The given name of the employee.</span></span>                        |
|<span data-ttu-id="b3e01-141">middleName</span><span class="sxs-lookup"><span data-stu-id="b3e01-141">middleName</span></span>          |<span data-ttu-id="b3e01-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-142">string</span></span>  |<span data-ttu-id="b3e01-143">O nome do meio do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-143">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="b3e01-144">surname</span><span class="sxs-lookup"><span data-stu-id="b3e01-144">surname</span></span>             |<span data-ttu-id="b3e01-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-145">string</span></span>  |<span data-ttu-id="b3e01-146">O sobrenome do funcionário</span><span class="sxs-lookup"><span data-stu-id="b3e01-146">The surname of the employee</span></span>                            |
|<span data-ttu-id="b3e01-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b3e01-147">jobTitle</span></span>            |<span data-ttu-id="b3e01-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-148">string</span></span>  |<span data-ttu-id="b3e01-149">O nome completo do funcionário</span><span class="sxs-lookup"><span data-stu-id="b3e01-149">The full name of the employee</span></span>                          |
|<span data-ttu-id="b3e01-150">address</span><span class="sxs-lookup"><span data-stu-id="b3e01-150">address</span></span>             |[<span data-ttu-id="b3e01-151">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="b3e01-151">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="b3e01-152">Especifica o endereço do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-152">Specifies the employee's address.</span></span> <span data-ttu-id="b3e01-153">Esse endereço aparecerá em todos os documentos de recursos do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-153">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="b3e01-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b3e01-154">phoneNumber</span></span>         |<span data-ttu-id="b3e01-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-155">string</span></span>  |<span data-ttu-id="b3e01-156">Especifica o número de telefone do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-156">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="b3e01-157">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="b3e01-157">mobilePhone</span></span>         |<span data-ttu-id="b3e01-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-158">string</span></span>  |<span data-ttu-id="b3e01-159">Especifica o número de telefone celular do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-159">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="b3e01-160">email</span><span class="sxs-lookup"><span data-stu-id="b3e01-160">email</span></span>               |<span data-ttu-id="b3e01-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-161">string</span></span>  |<span data-ttu-id="b3e01-162">Especifica o endereço de email do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-162">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="b3e01-163">personalEmail</span><span class="sxs-lookup"><span data-stu-id="b3e01-163">personalEmail</span></span>       |<span data-ttu-id="b3e01-164">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-164">string</span></span>  |<span data-ttu-id="b3e01-165">Especifica o endereço de email pessoal do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-165">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="b3e01-166">employmentDate</span><span class="sxs-lookup"><span data-stu-id="b3e01-166">employmentDate</span></span>      |<span data-ttu-id="b3e01-167">data</span><span class="sxs-lookup"><span data-stu-id="b3e01-167">date</span></span>    |<span data-ttu-id="b3e01-168">Especifica a data em que o funcionário começou a trabalhar para a empresa.</span><span class="sxs-lookup"><span data-stu-id="b3e01-168">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="b3e01-169">terminationDate</span><span class="sxs-lookup"><span data-stu-id="b3e01-169">terminationDate</span></span>     |<span data-ttu-id="b3e01-170">data</span><span class="sxs-lookup"><span data-stu-id="b3e01-170">date</span></span>    |<span data-ttu-id="b3e01-171">Especifica a data de término do funcionário, devido à aposentadoria ou à descarta, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="b3e01-171">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="b3e01-172">status</span><span class="sxs-lookup"><span data-stu-id="b3e01-172">status</span></span>              |<span data-ttu-id="b3e01-173">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b3e01-173">string</span></span>  |<span data-ttu-id="b3e01-174">Especifica o status do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-174">Specifies the employee's status.</span></span> <span data-ttu-id="b3e01-175">Os valores possíveis estão ativos, inativos ou terminados</span><span class="sxs-lookup"><span data-stu-id="b3e01-175">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="b3e01-176">birthDate</span><span class="sxs-lookup"><span data-stu-id="b3e01-176">birthDate</span></span>           |<span data-ttu-id="b3e01-177">data</span><span class="sxs-lookup"><span data-stu-id="b3e01-177">date</span></span>    |<span data-ttu-id="b3e01-178">Especifica a data de nascimento do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-178">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="b3e01-179">Panorama</span><span class="sxs-lookup"><span data-stu-id="b3e01-179">picture</span></span>             |<span data-ttu-id="b3e01-180">stream</span><span class="sxs-lookup"><span data-stu-id="b3e01-180">stream</span></span>  |<span data-ttu-id="b3e01-181">A imagem do funcionário.</span><span class="sxs-lookup"><span data-stu-id="b3e01-181">The employee picture.</span></span> <span data-ttu-id="b3e01-182">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="b3e01-182">Read-Only.</span></span>                       |
|<span data-ttu-id="b3e01-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3e01-183">lastModifiedDateTime</span></span>|<span data-ttu-id="b3e01-184">datetime</span><span class="sxs-lookup"><span data-stu-id="b3e01-184">datetime</span></span>|<span data-ttu-id="b3e01-185">O último DateTime que o funcionário foi modificado.</span><span class="sxs-lookup"><span data-stu-id="b3e01-185">The last datetime the employee was modified.</span></span> <span data-ttu-id="b3e01-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b3e01-186">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="b3e01-187">Relações</span><span class="sxs-lookup"><span data-stu-id="b3e01-187">Relationships</span></span>
<span data-ttu-id="b3e01-188">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b3e01-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3e01-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b3e01-189">JSON representation</span></span>

<span data-ttu-id="b3e01-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b3e01-190">Here is a JSON representation of the resource.</span></span>


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



