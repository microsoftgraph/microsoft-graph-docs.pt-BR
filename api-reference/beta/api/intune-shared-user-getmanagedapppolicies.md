---
title: Função getManagedAppPolicies
description: Obtém as restrições de aplicativo para um determinado usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36eb834668973a639eae64190791577e892c4494
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303885"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="f2aab-103">Função getManagedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="f2aab-103">getManagedAppPolicies function</span></span>

<span data-ttu-id="f2aab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2aab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2aab-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f2aab-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f2aab-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f2aab-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2aab-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f2aab-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2aab-108">Obtém as restrições de aplicativo para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="f2aab-108">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2aab-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f2aab-109">Prerequisites</span></span>

<span data-ttu-id="f2aab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2aab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2aab-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f2aab-112">Permission type</span></span>|<span data-ttu-id="f2aab-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f2aab-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2aab-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f2aab-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f2aab-115">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="f2aab-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f2aab-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2aab-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f2aab-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f2aab-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2aab-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f2aab-118">Not supported.</span></span>|
|<span data-ttu-id="f2aab-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f2aab-119">Application</span></span>||
| <span data-ttu-id="f2aab-120">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="f2aab-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="f2aab-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f2aab-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2aab-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f2aab-122">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="f2aab-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2aab-123">Request headers</span></span>

|<span data-ttu-id="f2aab-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f2aab-124">Header</span></span>|<span data-ttu-id="f2aab-125">Valor</span><span class="sxs-lookup"><span data-stu-id="f2aab-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2aab-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f2aab-126">Authorization</span></span>|<span data-ttu-id="f2aab-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f2aab-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2aab-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f2aab-128">Accept</span></span>|<span data-ttu-id="f2aab-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f2aab-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2aab-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f2aab-130">Request body</span></span>

<span data-ttu-id="f2aab-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f2aab-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2aab-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2aab-132">Response</span></span>

<span data-ttu-id="f2aab-133">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f2aab-133">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2aab-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f2aab-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2aab-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f2aab-135">Request</span></span>

<span data-ttu-id="f2aab-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f2aab-136">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="f2aab-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f2aab-137">Response</span></span>

<span data-ttu-id="f2aab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f2aab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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













