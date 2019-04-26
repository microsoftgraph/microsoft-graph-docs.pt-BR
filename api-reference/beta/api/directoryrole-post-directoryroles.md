---
title: Ativar directoryRole
description: Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário. Somente as funções de diretório administradores da empresa e usuários implícitos são ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente (directoryRoleTemplate).
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87579a801b148e29c3687e1fa93423b2ed3bd00b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326246"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="6d737-106">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="6d737-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d737-107">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="6d737-107">Activate a directory role.</span></span> <span data-ttu-id="6d737-108">Para ler uma função de diretório ou atualizar seus membros, primeiro ela deve ser ativada no locatário.</span><span class="sxs-lookup"><span data-stu-id="6d737-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="6d737-109">Somente as funções de diretório administradores da empresa e usuários implícitos são ativadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="6d737-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="6d737-110">Para acessar e atribuir membros a outra função de diretório, primeiro você deve ativá-lo com seu modelo de função de diretório correspondente ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="6d737-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="6d737-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="6d737-111">Permissions</span></span>
<span data-ttu-id="6d737-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d737-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d737-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d737-114">Permission type</span></span>      | <span data-ttu-id="6d737-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d737-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d737-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d737-116">Delegated (work or school account)</span></span> | <span data-ttu-id="6d737-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d737-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d737-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d737-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d737-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d737-119">Not supported.</span></span>    |
|<span data-ttu-id="6d737-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d737-120">Application</span></span> | <span data-ttu-id="6d737-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d737-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d737-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d737-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="6d737-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d737-123">Request headers</span></span>
| <span data-ttu-id="6d737-124">Nome</span><span class="sxs-lookup"><span data-stu-id="6d737-124">Name</span></span>       | <span data-ttu-id="6d737-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d737-125">Type</span></span> | <span data-ttu-id="6d737-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d737-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d737-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d737-127">Authorization</span></span>  | <span data-ttu-id="6d737-128">string</span><span class="sxs-lookup"><span data-stu-id="6d737-128">string</span></span>  | <span data-ttu-id="6d737-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d737-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d737-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d737-131">Request body</span></span>
<span data-ttu-id="6d737-132">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="6d737-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="6d737-133">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="6d737-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="6d737-134">Parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="6d737-134">Required parameter</span></span> | <span data-ttu-id="6d737-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d737-135">Type</span></span> | <span data-ttu-id="6d737-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d737-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="6d737-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="6d737-137">roleTemplateId</span></span> | <span data-ttu-id="6d737-138">string</span><span class="sxs-lookup"><span data-stu-id="6d737-138">string</span></span> | <span data-ttu-id="6d737-p105">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia. Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d737-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="6d737-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d737-141">Response</span></span>

<span data-ttu-id="6d737-142">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d737-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d737-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6d737-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d737-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d737-144">Request</span></span>
<span data-ttu-id="6d737-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d737-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json
Content-length: 153

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="6d737-146">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="6d737-146">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6d737-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d737-147">Response</span></span>
<span data-ttu-id="6d737-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6d737-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 175

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
