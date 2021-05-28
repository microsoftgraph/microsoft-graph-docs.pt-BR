---
title: tipo de recurso de funcionários
description: Um objeto de funcionário no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: eceea9e1811b61045c03fb8dc5d7710f33158ccc
ms.sourcegitcommit: a9a035e7cf7b500aebe5477c05361552e7c3a7ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52695970"
---
# <a name="employees-resource-type"></a><span data-ttu-id="3843a-103">tipo de recurso de funcionários</span><span class="sxs-lookup"><span data-stu-id="3843a-103">employees resource type</span></span>

<span data-ttu-id="3843a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3843a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3843a-105">Representa um funcionário no Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="3843a-105">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="3843a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3843a-106">Methods</span></span>

| <span data-ttu-id="3843a-107">Método</span><span class="sxs-lookup"><span data-stu-id="3843a-107">Method</span></span>                                              | <span data-ttu-id="3843a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3843a-108">Return Type</span></span>|<span data-ttu-id="3843a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3843a-109">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="3843a-110">Obter funcionários</span><span class="sxs-lookup"><span data-stu-id="3843a-110">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="3843a-111">employees</span><span class="sxs-lookup"><span data-stu-id="3843a-111">employees</span></span>  |<span data-ttu-id="3843a-112">Obter um objeto de funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-112">Get an employee object.</span></span>   |
|[<span data-ttu-id="3843a-113">Funcionários de postagem</span><span class="sxs-lookup"><span data-stu-id="3843a-113">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="3843a-114">employees</span><span class="sxs-lookup"><span data-stu-id="3843a-114">employees</span></span>  |<span data-ttu-id="3843a-115">Crie um objeto de funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-115">Create an employee object.</span></span>|
|[<span data-ttu-id="3843a-116">Corrigir funcionários</span><span class="sxs-lookup"><span data-stu-id="3843a-116">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="3843a-117">employees</span><span class="sxs-lookup"><span data-stu-id="3843a-117">employees</span></span>  |<span data-ttu-id="3843a-118">Atualizar um objeto de funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-118">Update an employee object.</span></span>|
|[<span data-ttu-id="3843a-119">Excluir funcionários</span><span class="sxs-lookup"><span data-stu-id="3843a-119">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="3843a-120">nenhuma</span><span class="sxs-lookup"><span data-stu-id="3843a-120">none</span></span>       |<span data-ttu-id="3843a-121">Excluir um objeto de funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-121">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3843a-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3843a-122">Properties</span></span>
| <span data-ttu-id="3843a-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3843a-123">Property</span></span>           | <span data-ttu-id="3843a-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="3843a-124">Type</span></span>   |<span data-ttu-id="3843a-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="3843a-125">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="3843a-126">id</span><span class="sxs-lookup"><span data-stu-id="3843a-126">id</span></span>                  |<span data-ttu-id="3843a-127">GUID</span><span class="sxs-lookup"><span data-stu-id="3843a-127">GUID</span></span>    |<span data-ttu-id="3843a-128">A ID do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-128">The employee ID.</span></span> <span data-ttu-id="3843a-129">Não editável.</span><span class="sxs-lookup"><span data-stu-id="3843a-129">Non-editable.</span></span>                         |
|<span data-ttu-id="3843a-130">number</span><span class="sxs-lookup"><span data-stu-id="3843a-130">number</span></span>              |<span data-ttu-id="3843a-131">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-131">string</span></span>  |<span data-ttu-id="3843a-132">O número do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-132">The employee number.</span></span> <span data-ttu-id="3843a-133">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="3843a-133">Read-Only.</span></span>                        |
|<span data-ttu-id="3843a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="3843a-134">displayName</span></span>         |<span data-ttu-id="3843a-135">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-135">string</span></span>  |<span data-ttu-id="3843a-136">O funcionário givenName + sobrenome.</span><span class="sxs-lookup"><span data-stu-id="3843a-136">The employee givenName + surname.</span></span> <span data-ttu-id="3843a-137">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="3843a-137">Read-Only.</span></span>           |
|<span data-ttu-id="3843a-138">givenName</span><span class="sxs-lookup"><span data-stu-id="3843a-138">givenName</span></span>           |<span data-ttu-id="3843a-139">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-139">string</span></span>  |<span data-ttu-id="3843a-140">O nome dado do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-140">The given name of the employee.</span></span>                        |
|<span data-ttu-id="3843a-141">middleName</span><span class="sxs-lookup"><span data-stu-id="3843a-141">middleName</span></span>          |<span data-ttu-id="3843a-142">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-142">string</span></span>  |<span data-ttu-id="3843a-143">O nome do meio do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-143">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="3843a-144">surname</span><span class="sxs-lookup"><span data-stu-id="3843a-144">surname</span></span>             |<span data-ttu-id="3843a-145">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-145">string</span></span>  |<span data-ttu-id="3843a-146">O sobrenome do funcionário</span><span class="sxs-lookup"><span data-stu-id="3843a-146">The surname of the employee</span></span>                            |
|<span data-ttu-id="3843a-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="3843a-147">jobTitle</span></span>            |<span data-ttu-id="3843a-148">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-148">string</span></span>  |<span data-ttu-id="3843a-149">O cargo do funcionário</span><span class="sxs-lookup"><span data-stu-id="3843a-149">The job title of the employee</span></span>                          |
|<span data-ttu-id="3843a-150">address</span><span class="sxs-lookup"><span data-stu-id="3843a-150">address</span></span>             |[<span data-ttu-id="3843a-151">NAV. PostalAddress</span><span class="sxs-lookup"><span data-stu-id="3843a-151">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="3843a-152">Especifica o endereço do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-152">Specifies the employee's address.</span></span> <span data-ttu-id="3843a-153">Esse endereço aparecerá em todos os documentos de recursos do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-153">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="3843a-154">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="3843a-154">phoneNumber</span></span>         |<span data-ttu-id="3843a-155">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-155">string</span></span>  |<span data-ttu-id="3843a-156">Especifica o número de telefone do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-156">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="3843a-157">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="3843a-157">mobilePhone</span></span>         |<span data-ttu-id="3843a-158">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-158">string</span></span>  |<span data-ttu-id="3843a-159">Especifica o número de telefone celular do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-159">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="3843a-160">email</span><span class="sxs-lookup"><span data-stu-id="3843a-160">email</span></span>               |<span data-ttu-id="3843a-161">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-161">string</span></span>  |<span data-ttu-id="3843a-162">Especifica o endereço de email do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-162">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="3843a-163">personalEmail</span><span class="sxs-lookup"><span data-stu-id="3843a-163">personalEmail</span></span>       |<span data-ttu-id="3843a-164">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-164">string</span></span>  |<span data-ttu-id="3843a-165">Especifica o endereço de email pessoal do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-165">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="3843a-166">employmentDate</span><span class="sxs-lookup"><span data-stu-id="3843a-166">employmentDate</span></span>      |<span data-ttu-id="3843a-167">data</span><span class="sxs-lookup"><span data-stu-id="3843a-167">date</span></span>    |<span data-ttu-id="3843a-168">Especifica a data em que o funcionário começou a trabalhar para a empresa.</span><span class="sxs-lookup"><span data-stu-id="3843a-168">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="3843a-169">terminationDate</span><span class="sxs-lookup"><span data-stu-id="3843a-169">terminationDate</span></span>     |<span data-ttu-id="3843a-170">data</span><span class="sxs-lookup"><span data-stu-id="3843a-170">date</span></span>    |<span data-ttu-id="3843a-171">Especifica a data em que o funcionário foi encerrado, devido à aposentadoria ou à demissão, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="3843a-171">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="3843a-172">status</span><span class="sxs-lookup"><span data-stu-id="3843a-172">status</span></span>              |<span data-ttu-id="3843a-173">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3843a-173">string</span></span>  |<span data-ttu-id="3843a-174">Especifica o status do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-174">Specifies the employee's status.</span></span> <span data-ttu-id="3843a-175">Os valores possíveis são Active, Inactive ou Terminated</span><span class="sxs-lookup"><span data-stu-id="3843a-175">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="3843a-176">birthDate</span><span class="sxs-lookup"><span data-stu-id="3843a-176">birthDate</span></span>           |<span data-ttu-id="3843a-177">data</span><span class="sxs-lookup"><span data-stu-id="3843a-177">date</span></span>    |<span data-ttu-id="3843a-178">Especifica a data de nascimento do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-178">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="3843a-179">picture</span><span class="sxs-lookup"><span data-stu-id="3843a-179">picture</span></span>             |<span data-ttu-id="3843a-180">stream</span><span class="sxs-lookup"><span data-stu-id="3843a-180">stream</span></span>  |<span data-ttu-id="3843a-181">A imagem do funcionário.</span><span class="sxs-lookup"><span data-stu-id="3843a-181">The employee picture.</span></span> <span data-ttu-id="3843a-182">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="3843a-182">Read-Only.</span></span>                       |
|<span data-ttu-id="3843a-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3843a-183">lastModifiedDateTime</span></span>|<span data-ttu-id="3843a-184">datetime</span><span class="sxs-lookup"><span data-stu-id="3843a-184">datetime</span></span>|<span data-ttu-id="3843a-185">A última data em que o funcionário foi modificado.</span><span class="sxs-lookup"><span data-stu-id="3843a-185">The last datetime the employee was modified.</span></span> <span data-ttu-id="3843a-186">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3843a-186">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="3843a-187">Relações</span><span class="sxs-lookup"><span data-stu-id="3843a-187">Relationships</span></span>
<span data-ttu-id="3843a-188">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3843a-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3843a-189">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3843a-189">JSON representation</span></span>

<span data-ttu-id="3843a-190">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3843a-190">Here is a JSON representation of the resource.</span></span>


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



