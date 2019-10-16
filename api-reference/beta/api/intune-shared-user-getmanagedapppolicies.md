---
title: Função getManagedAppPolicies
description: Obtém as restrições de aplicativo para um determinado usuário.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a0a6c36c0d25853a0709a50c8eddb45d29a74cd9
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536963"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="3319d-103">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="3319d-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="3319d-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3319d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3319d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3319d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3319d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3319d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3319d-107">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="3319d-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3319d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3319d-108">Prerequisites</span></span>

<span data-ttu-id="3319d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3319d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3319d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3319d-111">Permission type</span></span>|<span data-ttu-id="3319d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3319d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3319d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3319d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="3319d-114">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="3319d-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3319d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3319d-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="3319d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3319d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3319d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3319d-117">Not supported.</span></span>|
|<span data-ttu-id="3319d-118">Application</span><span class="sxs-lookup"><span data-stu-id="3319d-118">Application</span></span>||
| <span data-ttu-id="3319d-119">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="3319d-119">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="3319d-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="3319d-120">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3319d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3319d-121">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="3319d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3319d-122">Request headers</span></span>

|<span data-ttu-id="3319d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3319d-123">Header</span></span>|<span data-ttu-id="3319d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3319d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3319d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3319d-125">Authorization</span></span>|<span data-ttu-id="3319d-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3319d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3319d-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3319d-127">Accept</span></span>|<span data-ttu-id="3319d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3319d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3319d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3319d-129">Request body</span></span>

<span data-ttu-id="3319d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3319d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3319d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3319d-131">Response</span></span>

<span data-ttu-id="3319d-132">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3319d-132">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3319d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3319d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3319d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3319d-134">Request</span></span>

<span data-ttu-id="3319d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3319d-135">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="3319d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3319d-136">Response</span></span>

<span data-ttu-id="3319d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3319d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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












