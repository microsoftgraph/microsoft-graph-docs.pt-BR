---
title: função isManagedAppUserBlocked
description: Obtém o estado bloqueado de um usuário de aplicativo gerenciado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 07f7295a3096c5c3dd11c6f4903d51b14d67aeb2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148943"
---
# <a name="ismanagedappuserblocked-function"></a><span data-ttu-id="6671a-103">função isManagedAppUserBlocked</span><span class="sxs-lookup"><span data-stu-id="6671a-103">isManagedAppUserBlocked function</span></span>

<span data-ttu-id="6671a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6671a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6671a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6671a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6671a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6671a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6671a-107">Obtém o estado bloqueado de um usuário de aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6671a-107">Gets the blocked state of a managed app user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6671a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6671a-108">Prerequisites</span></span>
<span data-ttu-id="6671a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6671a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6671a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6671a-111">Permission type</span></span>|<span data-ttu-id="6671a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6671a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6671a-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6671a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6671a-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6671a-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6671a-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6671a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6671a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6671a-116">Not supported.</span></span>|
|<span data-ttu-id="6671a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6671a-117">Application</span></span>|<span data-ttu-id="6671a-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6671a-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6671a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6671a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/isManagedAppUserBlocked
```

## <a name="request-headers"></a><span data-ttu-id="6671a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6671a-120">Request headers</span></span>
|<span data-ttu-id="6671a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6671a-121">Header</span></span>|<span data-ttu-id="6671a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6671a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6671a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6671a-123">Authorization</span></span>|<span data-ttu-id="6671a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6671a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6671a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6671a-125">Accept</span></span>|<span data-ttu-id="6671a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6671a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6671a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6671a-127">Request body</span></span>
<span data-ttu-id="6671a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6671a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6671a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6671a-129">Response</span></span>
<span data-ttu-id="6671a-130">Se tiver êxito, essa função retornará o código resposta `200 OK` e um Booliano no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6671a-130">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6671a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6671a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6671a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6671a-132">Request</span></span>
<span data-ttu-id="6671a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6671a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/isManagedAppUserBlocked
```

### <a name="response"></a><span data-ttu-id="6671a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6671a-134">Response</span></span>
<span data-ttu-id="6671a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6671a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```




