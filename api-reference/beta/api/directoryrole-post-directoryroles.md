---
title: Ativar directoryRole
description: Ative uma função de diretório. Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino. Somente os administradores da empresa e as funções de diretório de usuários implícitas serão ativadas por padrão. Para acessar e atribuir membros a outra função de diretório, você deve ativá-lo com o modelo de função correspondente do diretório (directoryRoleTemplate).
localization_priority: Normal
ms.openlocfilehash: 6045b4307b571d84ac28467af21f7aa89b6ee7fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894387"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="7e8e5-106">Ativar directoryRole</span><span class="sxs-lookup"><span data-stu-id="7e8e5-106">Activate directoryRole</span></span>

> <span data-ttu-id="7e8e5-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e8e5-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e8e5-109">Ative uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-109">Activate a directory role.</span></span> <span data-ttu-id="7e8e5-110">Para ler uma função de diretório ou atualizar seus membros, ele deve primeiro ser ativado no inquilino.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="7e8e5-111">Somente os administradores da empresa e as funções de diretório de usuários implícitas serão ativadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-111">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="7e8e5-112">Para acessar e atribuir membros a outra função de diretório, você deve ativá-lo com o modelo de função correspondente do diretório ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="7e8e5-112">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="7e8e5-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="7e8e5-113">Permissions</span></span>
<span data-ttu-id="7e8e5-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e8e5-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e8e5-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e8e5-116">Permission type</span></span>      | <span data-ttu-id="7e8e5-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e8e5-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e8e5-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e8e5-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7e8e5-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7e8e5-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7e8e5-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e8e5-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e8e5-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-121">Not supported.</span></span>    |
|<span data-ttu-id="7e8e5-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e8e5-122">Application</span></span> | <span data-ttu-id="7e8e5-123">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e8e5-123">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e8e5-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e8e5-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="7e8e5-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e8e5-125">Request headers</span></span>
| <span data-ttu-id="7e8e5-126">Nome</span><span class="sxs-lookup"><span data-stu-id="7e8e5-126">Name</span></span>       | <span data-ttu-id="7e8e5-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e8e5-127">Type</span></span> | <span data-ttu-id="7e8e5-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e8e5-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7e8e5-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e8e5-129">Authorization</span></span>  | <span data-ttu-id="7e8e5-130">string</span><span class="sxs-lookup"><span data-stu-id="7e8e5-130">string</span></span>  | <span data-ttu-id="7e8e5-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e8e5-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e8e5-133">Request body</span></span>
<span data-ttu-id="7e8e5-134">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="7e8e5-134">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="7e8e5-135">A tabela a seguir mostra as propriedades que são necessárias ao ativar uma função de diretório.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-135">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="7e8e5-136">Parâmetro obrigatório</span><span class="sxs-lookup"><span data-stu-id="7e8e5-136">Required parameter</span></span> | <span data-ttu-id="7e8e5-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e8e5-137">Type</span></span> | <span data-ttu-id="7e8e5-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e8e5-138">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="7e8e5-139">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="7e8e5-139">roleTemplateId</span></span> | <span data-ttu-id="7e8e5-140">string</span><span class="sxs-lookup"><span data-stu-id="7e8e5-140">string</span></span> | <span data-ttu-id="7e8e5-p106">A ID do [directoryRoleTemplate](../resources/directoryroletemplate.md) em que a função se baseia. Esta é a única propriedade que pode ser especificada na solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-p106">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="7e8e5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e8e5-143">Response</span></span>

<span data-ttu-id="7e8e5-144">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [directoryRole](../resources/directoryrole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e8e5-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e8e5-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e8e5-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e8e5-146">Request</span></span>
<span data-ttu-id="7e8e5-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-147">Here is an example of the request.</span></span>
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
<span data-ttu-id="7e8e5-148">No corpo da solicitação, forneça uma representação JSON do objeto [directoryRole](../resources/directoryrole.md).</span><span class="sxs-lookup"><span data-stu-id="7e8e5-148">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7e8e5-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e8e5-149">Response</span></span>
<span data-ttu-id="7e8e5-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e8e5-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
