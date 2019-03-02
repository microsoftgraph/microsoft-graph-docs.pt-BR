---
title: tipo de recurso Employees
description: Um objeto Employee no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 865da0c1e1256e2ba2a25902e37a00da9081eedf
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366652"
---
# <a name="employees-resource-type"></a><span data-ttu-id="c2a89-103">tipo de recurso Employees</span><span class="sxs-lookup"><span data-stu-id="c2a89-103">employees resource type</span></span>
<span data-ttu-id="c2a89-104">Representa um funcionário no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="c2a89-104">Represents an employee in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="c2a89-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c2a89-105">Methods</span></span>

| <span data-ttu-id="c2a89-106">Método</span><span class="sxs-lookup"><span data-stu-id="c2a89-106">Method</span></span>                                              | <span data-ttu-id="c2a89-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c2a89-107">Return Type</span></span>|<span data-ttu-id="c2a89-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2a89-108">Description</span></span>               |
|:----------------------------------------------------|:-----------|:-------------------------|
|[<span data-ttu-id="c2a89-109">Obter funcionários</span><span class="sxs-lookup"><span data-stu-id="c2a89-109">Get employees</span></span>](../api/dynamics-employee-get.md)      |<span data-ttu-id="c2a89-110">dos</span><span class="sxs-lookup"><span data-stu-id="c2a89-110">employees</span></span>  |<span data-ttu-id="c2a89-111">Obter um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="c2a89-111">Get an employee object.</span></span>   |
|[<span data-ttu-id="c2a89-112">Postar funcionários</span><span class="sxs-lookup"><span data-stu-id="c2a89-112">Post employees</span></span>](../api/dynamics-create-employee.md)  |<span data-ttu-id="c2a89-113">dos</span><span class="sxs-lookup"><span data-stu-id="c2a89-113">employees</span></span>  |<span data-ttu-id="c2a89-114">Criar um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="c2a89-114">Create an employee object.</span></span>|
|[<span data-ttu-id="c2a89-115">Patch funcionários</span><span class="sxs-lookup"><span data-stu-id="c2a89-115">Patch employees</span></span>](../api/dynamics-employee-update.md) |<span data-ttu-id="c2a89-116">dos</span><span class="sxs-lookup"><span data-stu-id="c2a89-116">employees</span></span>  |<span data-ttu-id="c2a89-117">Atualizar um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="c2a89-117">Update an employee object.</span></span>|
|[<span data-ttu-id="c2a89-118">Excluir funcionários</span><span class="sxs-lookup"><span data-stu-id="c2a89-118">Delete employees</span></span>](../api/dynamics-employee-delete.md)|<span data-ttu-id="c2a89-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c2a89-119">none</span></span>       |<span data-ttu-id="c2a89-120">Excluir um objeto Employee.</span><span class="sxs-lookup"><span data-stu-id="c2a89-120">Delete an employee object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c2a89-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2a89-121">Properties</span></span>
| <span data-ttu-id="c2a89-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2a89-122">Property</span></span>           | <span data-ttu-id="c2a89-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2a89-123">Type</span></span>   |<span data-ttu-id="c2a89-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2a89-124">Description</span></span>                                            |
|:-------------------|:-------|:------------------------------------------------------|
|<span data-ttu-id="c2a89-125">id</span><span class="sxs-lookup"><span data-stu-id="c2a89-125">id</span></span>                  |<span data-ttu-id="c2a89-126">GUID</span><span class="sxs-lookup"><span data-stu-id="c2a89-126">GUID</span></span>    |<span data-ttu-id="c2a89-127">A ID do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-127">The employee ID.</span></span> <span data-ttu-id="c2a89-128">Não editável.</span><span class="sxs-lookup"><span data-stu-id="c2a89-128">Non-editable.</span></span>                         |
|<span data-ttu-id="c2a89-129">number</span><span class="sxs-lookup"><span data-stu-id="c2a89-129">number</span></span>              |<span data-ttu-id="c2a89-130">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-130">string</span></span>  |<span data-ttu-id="c2a89-131">O número do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-131">The employee number.</span></span> <span data-ttu-id="c2a89-132">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c2a89-132">Read-Only.</span></span>                        |
|<span data-ttu-id="c2a89-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c2a89-133">displayName</span></span>         |<span data-ttu-id="c2a89-134">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-134">string</span></span>  |<span data-ttu-id="c2a89-135">O funcionário de atribuído + sobrenome.</span><span class="sxs-lookup"><span data-stu-id="c2a89-135">The employee givenName + surname.</span></span> <span data-ttu-id="c2a89-136">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c2a89-136">Read-Only.</span></span>           |
|<span data-ttu-id="c2a89-137">givenName</span><span class="sxs-lookup"><span data-stu-id="c2a89-137">givenName</span></span>           |<span data-ttu-id="c2a89-138">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-138">string</span></span>  |<span data-ttu-id="c2a89-139">O nome fornecido do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-139">The given name of the employee.</span></span>                        |
|<span data-ttu-id="c2a89-140">middleName</span><span class="sxs-lookup"><span data-stu-id="c2a89-140">middleName</span></span>          |<span data-ttu-id="c2a89-141">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-141">string</span></span>  |<span data-ttu-id="c2a89-142">O nome do meio do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-142">The middle name of the employee.</span></span>                       |
|<span data-ttu-id="c2a89-143">surname</span><span class="sxs-lookup"><span data-stu-id="c2a89-143">surname</span></span>             |<span data-ttu-id="c2a89-144">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-144">string</span></span>  |<span data-ttu-id="c2a89-145">O sobrenome do funcionário</span><span class="sxs-lookup"><span data-stu-id="c2a89-145">The surname of the employee</span></span>                            |
|<span data-ttu-id="c2a89-146">jobTitle</span><span class="sxs-lookup"><span data-stu-id="c2a89-146">jobTitle</span></span>            |<span data-ttu-id="c2a89-147">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-147">string</span></span>  |<span data-ttu-id="c2a89-148">O nome completo do funcionário</span><span class="sxs-lookup"><span data-stu-id="c2a89-148">The full name of the employee</span></span>                          |
|<span data-ttu-id="c2a89-149">address</span><span class="sxs-lookup"><span data-stu-id="c2a89-149">address</span></span>             |[<span data-ttu-id="c2a89-150">Extra. Address</span><span class="sxs-lookup"><span data-stu-id="c2a89-150">NAV.PostalAddress</span></span>](../resources/dynamics-complextypes.md)|<span data-ttu-id="c2a89-151">Especifica o endereço do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-151">Specifies the employee's address.</span></span> <span data-ttu-id="c2a89-152">Esse endereço aparecerá em todos os documentos de recursos do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-152">This address will appear on all resource documents for the employee.</span></span>|
|<span data-ttu-id="c2a89-153">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="c2a89-153">phoneNumber</span></span>         |<span data-ttu-id="c2a89-154">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-154">string</span></span>  |<span data-ttu-id="c2a89-155">Especifica o número de telefone do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-155">Specifies the employee's telephone number.</span></span>             |
|<span data-ttu-id="c2a89-156">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="c2a89-156">mobilePhone</span></span>         |<span data-ttu-id="c2a89-157">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-157">string</span></span>  |<span data-ttu-id="c2a89-158">Especifica o número de telefone celular do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-158">Specifies the employee's mobile telephone number.</span></span>      |
|<span data-ttu-id="c2a89-159">email</span><span class="sxs-lookup"><span data-stu-id="c2a89-159">email</span></span>               |<span data-ttu-id="c2a89-160">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-160">string</span></span>  |<span data-ttu-id="c2a89-161">Especifica o endereço de email do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-161">Specifies the employee's email address.</span></span>                |
|<span data-ttu-id="c2a89-162">personalEmail</span><span class="sxs-lookup"><span data-stu-id="c2a89-162">personalEmail</span></span>       |<span data-ttu-id="c2a89-163">string</span><span class="sxs-lookup"><span data-stu-id="c2a89-163">string</span></span>  |<span data-ttu-id="c2a89-164">Especifica o endereço de email pessoal do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-164">Specifies the employee's personal email address.</span></span>       |
|<span data-ttu-id="c2a89-165">employmentDate</span><span class="sxs-lookup"><span data-stu-id="c2a89-165">employmentDate</span></span>      |<span data-ttu-id="c2a89-166">data</span><span class="sxs-lookup"><span data-stu-id="c2a89-166">date</span></span>    |<span data-ttu-id="c2a89-167">Especifica a data em que o funcionário começou a trabalhar para a empresa.</span><span class="sxs-lookup"><span data-stu-id="c2a89-167">Specifies the date when the employee began to work for the company.</span></span>|
|<span data-ttu-id="c2a89-168">terminationDate</span><span class="sxs-lookup"><span data-stu-id="c2a89-168">terminationDate</span></span>     |<span data-ttu-id="c2a89-169">data</span><span class="sxs-lookup"><span data-stu-id="c2a89-169">date</span></span>    |<span data-ttu-id="c2a89-170">Especifica a data de término do funcionário, devido à aposentadoria ou à descarta, por exemplo.</span><span class="sxs-lookup"><span data-stu-id="c2a89-170">Specifies the date when the employee was terminated, due to retirement or dismissal, for example.</span></span>|
|<span data-ttu-id="c2a89-171">status</span><span class="sxs-lookup"><span data-stu-id="c2a89-171">status</span></span>              |<span data-ttu-id="c2a89-172">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2a89-172">string</span></span>  |<span data-ttu-id="c2a89-173">Especifica o status do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-173">Specifies the employee's status.</span></span> <span data-ttu-id="c2a89-174">Os valores possíveis estão ativos, inativos ou terminados</span><span class="sxs-lookup"><span data-stu-id="c2a89-174">Possible values are Active, Inactive or Terminated</span></span>|
|<span data-ttu-id="c2a89-175">birthDate</span><span class="sxs-lookup"><span data-stu-id="c2a89-175">birthDate</span></span>           |<span data-ttu-id="c2a89-176">data</span><span class="sxs-lookup"><span data-stu-id="c2a89-176">date</span></span>    |<span data-ttu-id="c2a89-177">Especifica a data de nascimento do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-177">Specifies the employee's date of birth.</span></span>                |
|<span data-ttu-id="c2a89-178">Panorama</span><span class="sxs-lookup"><span data-stu-id="c2a89-178">picture</span></span>             |<span data-ttu-id="c2a89-179">stream</span><span class="sxs-lookup"><span data-stu-id="c2a89-179">stream</span></span>  |<span data-ttu-id="c2a89-180">A imagem do funcionário.</span><span class="sxs-lookup"><span data-stu-id="c2a89-180">The employee picture.</span></span> <span data-ttu-id="c2a89-181">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c2a89-181">Read-Only.</span></span>                       |
|<span data-ttu-id="c2a89-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2a89-182">lastModifiedDateTime</span></span>|<span data-ttu-id="c2a89-183">DateTime</span><span class="sxs-lookup"><span data-stu-id="c2a89-183">datetime</span></span>|<span data-ttu-id="c2a89-184">O último DateTime que o funcionário foi modificado.</span><span class="sxs-lookup"><span data-stu-id="c2a89-184">The last datetime the employee was modified.</span></span> <span data-ttu-id="c2a89-185">Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c2a89-185">Read-Only.</span></span>|  


## <a name="relationships"></a><span data-ttu-id="c2a89-186">Relações</span><span class="sxs-lookup"><span data-stu-id="c2a89-186">Relationships</span></span>
<span data-ttu-id="c2a89-187">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2a89-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2a89-188">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2a89-188">JSON representation</span></span>

<span data-ttu-id="c2a89-189">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2a89-189">Here is a JSON representation of the resource.</span></span>


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

