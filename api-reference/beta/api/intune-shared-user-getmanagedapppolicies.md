---
title: Função getManagedAppPolicies
description: Obtém as restrições de aplicativo para um determinado usuário.
author: tfitzmac
ms.openlocfilehash: 9b0729e986a7ab3434d2682d157e45f543d558a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354793"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="dd4ee-103">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="dd4ee-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="dd4ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd4ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dd4ee-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd4ee-107">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd4ee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dd4ee-108">Prerequisites</span></span>

<span data-ttu-id="dd4ee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dd4ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd4ee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dd4ee-111">Permission type</span></span>|<span data-ttu-id="dd4ee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dd4ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd4ee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dd4ee-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dd4ee-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="dd4ee-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="dd4ee-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dd4ee-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dd4ee-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dd4ee-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd4ee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-117">Not supported.</span></span>|
|<span data-ttu-id="dd4ee-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dd4ee-118">Application</span></span>|<span data-ttu-id="dd4ee-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd4ee-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dd4ee-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="dd4ee-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dd4ee-121">Request headers</span></span>

|<span data-ttu-id="dd4ee-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dd4ee-122">Header</span></span>|<span data-ttu-id="dd4ee-123">Valor</span><span class="sxs-lookup"><span data-stu-id="dd4ee-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd4ee-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="dd4ee-124">Authorization</span></span>|<span data-ttu-id="dd4ee-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd4ee-126">Accept</span><span class="sxs-lookup"><span data-stu-id="dd4ee-126">Accept</span></span>|<span data-ttu-id="dd4ee-127">application/json</span><span class="sxs-lookup"><span data-stu-id="dd4ee-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd4ee-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dd4ee-128">Request body</span></span>

<span data-ttu-id="dd4ee-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd4ee-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd4ee-130">Response</span></span>

<span data-ttu-id="dd4ee-131">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd4ee-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dd4ee-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd4ee-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dd4ee-133">Request</span></span>

<span data-ttu-id="dd4ee-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="dd4ee-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="dd4ee-135">Response</span></span>

<span data-ttu-id="dd4ee-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dd4ee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```






