---
title: Obter membro
description: Use essa API para obter um determinado membro (usuário ou grupo) em uma unidade administrativa.
ms.openlocfilehash: 741a24434056783c3f008de6fb7694082b393092
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035953"
---
# <a name="get-a-member"></a><span data-ttu-id="3eb1d-103">Obter membro</span><span class="sxs-lookup"><span data-stu-id="3eb1d-103">Get a member</span></span>

> <span data-ttu-id="3eb1d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eb1d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3eb1d-106">Use essa API para obter um determinado membro (usuário ou grupo) em uma unidade administrativa.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-106">Use this API to get a specific member (user or group) in an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="3eb1d-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="3eb1d-107">Permissions</span></span>
<span data-ttu-id="3eb1d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3eb1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3eb1d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3eb1d-110">Permission type</span></span>      | <span data-ttu-id="3eb1d-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3eb1d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3eb1d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3eb1d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3eb1d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3eb1d-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3eb1d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3eb1d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3eb1d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-115">Not supported.</span></span>    |
|<span data-ttu-id="3eb1d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3eb1d-116">Application</span></span> | <span data-ttu-id="3eb1d-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eb1d-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3eb1d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3eb1d-118">HTTP request</span></span>

```http
GET /administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3eb1d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb1d-119">Request headers</span></span>
| <span data-ttu-id="3eb1d-120">Nome</span><span class="sxs-lookup"><span data-stu-id="3eb1d-120">Name</span></span>      |<span data-ttu-id="3eb1d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3eb1d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3eb1d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3eb1d-122">Authorization</span></span>  | <span data-ttu-id="3eb1d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3eb1d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb1d-125">Request body</span></span>
<span data-ttu-id="3eb1d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3eb1d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eb1d-127">Response</span></span>

<span data-ttu-id="3eb1d-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto de [usuário](../resources/user.md) ou [grupo](../resources/group.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-128">If successful, this method returns a `200 OK` response code and a [user](../resources/user.md) or [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eb1d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3eb1d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3eb1d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3eb1d-130">Request</span></span>
<span data-ttu-id="3eb1d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-131">Here is an example of the request.</span></span>

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/{id}
```

##### <a name="response"></a><span data-ttu-id="3eb1d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3eb1d-132">Response</span></span>
<span data-ttu-id="3eb1d-133">Aqui está um exemplo do respone.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-133">Here is an example of the respone.</span></span> <span data-ttu-id="3eb1d-134">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3eb1d-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3eb1d-135">All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "@odata.type":"#microsoft.graph.user",
  "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
  "accountEnabled":true,
  "businessPhones":[],
  "companyName":null,
  "displayName":"Demo User"
}
```