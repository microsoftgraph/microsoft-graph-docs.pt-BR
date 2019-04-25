---
title: Obter organização
description: Leia as propriedades e as relações do objeto organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 534dc20db95555fde23908b5d073a3846805896a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582553"
---
# <a name="get-organization"></a><span data-ttu-id="d582d-103">Obter organização</span><span class="sxs-lookup"><span data-stu-id="d582d-103">Get organization</span></span>

> <span data-ttu-id="d582d-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d582d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d582d-105">Leia as propriedades e as relações do objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="d582d-105">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d582d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d582d-106">Prerequisites</span></span>
<span data-ttu-id="d582d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d582d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d582d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d582d-109">Permission type</span></span>|<span data-ttu-id="d582d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d582d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d582d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d582d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d582d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d582d-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d582d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d582d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d582d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d582d-114">Not supported.</span></span>|
|<span data-ttu-id="d582d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d582d-115">Application</span></span>|<span data-ttu-id="d582d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d582d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d582d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d582d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /organization/{organizationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d582d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d582d-118">Optional query parameters</span></span>
<span data-ttu-id="d582d-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d582d-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d582d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d582d-120">Request headers</span></span>
|<span data-ttu-id="d582d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d582d-121">Header</span></span>|<span data-ttu-id="d582d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d582d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d582d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d582d-123">Authorization</span></span>|<span data-ttu-id="d582d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d582d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d582d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d582d-125">Accept</span></span>|<span data-ttu-id="d582d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d582d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d582d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d582d-127">Request body</span></span>
<span data-ttu-id="d582d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d582d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d582d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d582d-129">Response</span></span>
<span data-ttu-id="d582d-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d582d-130">If successful, this method returns a `200 OK` response code and [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d582d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d582d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d582d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d582d-132">Request</span></span>
<span data-ttu-id="d582d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d582d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/organization/{organizationId}
```

### <a name="response"></a><span data-ttu-id="d582d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d582d-134">Response</span></span>
<span data-ttu-id="d582d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d582d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "value": {
    "@odata.type": "#microsoft.graph.organization",
    "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
    "mobileDeviceManagementAuthority": "intune"
  }
}
```



