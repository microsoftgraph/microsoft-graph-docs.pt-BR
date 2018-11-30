---
title: Excluir usuário
description: Exclui usuário.
ms.openlocfilehash: 94c9909ef64f5b358c7e14d4d201a081db584851
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034146"
---
# <a name="delete-user"></a><span data-ttu-id="c9c99-103">Excluir usuário</span><span class="sxs-lookup"><span data-stu-id="c9c99-103">Delete user</span></span>

> <span data-ttu-id="c9c99-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9c99-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9c99-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9c99-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9c99-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c9c99-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9c99-107">Exclui [usuário](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="c9c99-107">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c9c99-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c9c99-108">Prerequisites</span></span>
<span data-ttu-id="c9c99-109">Uma das seguintes permissões é necessário chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="c9c99-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c9c99-110">Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9c99-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="c9c99-111">A permissão específica necessária depende de contexto.</span><span class="sxs-lookup"><span data-stu-id="c9c99-111">The specific permission required depends on context.</span></span>

|<span data-ttu-id="c9c99-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c9c99-112">Permission type</span></span>|<span data-ttu-id="c9c99-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c9c99-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9c99-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c9c99-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c9c99-115">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="c9c99-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="c9c99-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c99-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="c9c99-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="c9c99-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="c9c99-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c99-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="c9c99-119">&nbsp;&nbsp; **Onboarding**</span><span class="sxs-lookup"><span data-stu-id="c9c99-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="c9c99-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c99-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="c9c99-121">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="c9c99-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="c9c99-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9c99-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c9c99-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c9c99-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9c99-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9c99-124">Not supported.</span></span>|
|<span data-ttu-id="c9c99-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c9c99-125">Application</span></span>|<span data-ttu-id="c9c99-126">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c9c99-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9c99-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c9c99-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="c9c99-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c9c99-128">Request headers</span></span>

|<span data-ttu-id="c9c99-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c9c99-129">Header</span></span>|<span data-ttu-id="c9c99-130">Valor</span><span class="sxs-lookup"><span data-stu-id="c9c99-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9c99-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="c9c99-131">Authorization</span></span>|<span data-ttu-id="c9c99-132">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c9c99-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9c99-133">Accept</span><span class="sxs-lookup"><span data-stu-id="c9c99-133">Accept</span></span>|<span data-ttu-id="c9c99-134">application/json</span><span class="sxs-lookup"><span data-stu-id="c9c99-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9c99-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c9c99-135">Request body</span></span>

<span data-ttu-id="c9c99-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c9c99-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9c99-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9c99-137">Response</span></span>

<span data-ttu-id="c9c99-138">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c9c99-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c9c99-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9c99-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9c99-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9c99-140">Request</span></span>

<span data-ttu-id="c9c99-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c9c99-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/beta/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="c9c99-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9c99-142">Response</span></span>

<span data-ttu-id="c9c99-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c9c99-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



