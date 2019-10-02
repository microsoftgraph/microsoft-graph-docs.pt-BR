---
title: função getManagedAppDiagnosticStatuses
description: Obtém diagnóstico do status de validação para um determinado usuário.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3ff023842e487997489ace66bad68b51c686cd91
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361291"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="a6c44-103">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="a6c44-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="a6c44-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6c44-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6c44-105">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="a6c44-105">Gets diagnostics validation status for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6c44-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6c44-106">Prerequisites</span></span>
<span data-ttu-id="a6c44-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c44-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6c44-109">Permission type</span></span>|<span data-ttu-id="a6c44-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a6c44-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6c44-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6c44-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a6c44-112">_varia por contexto_</span><span class="sxs-lookup"><span data-stu-id="a6c44-112">_varies by context_</span></span>|
| <span data-ttu-id="a6c44-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="a6c44-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="a6c44-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6c44-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="a6c44-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6c44-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6c44-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6c44-116">Not supported.</span></span>|
|<span data-ttu-id="a6c44-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6c44-117">Application</span></span>|<span data-ttu-id="a6c44-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6c44-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6c44-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6c44-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a6c44-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c44-120">Request headers</span></span>
|<span data-ttu-id="a6c44-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6c44-121">Header</span></span>|<span data-ttu-id="a6c44-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a6c44-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6c44-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6c44-123">Authorization</span></span>|<span data-ttu-id="a6c44-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6c44-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6c44-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6c44-125">Accept</span></span>|<span data-ttu-id="a6c44-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6c44-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c44-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c44-127">Request body</span></span>
<span data-ttu-id="a6c44-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6c44-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6c44-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c44-129">Response</span></span>
<span data-ttu-id="a6c44-130">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6c44-130">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c44-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6c44-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6c44-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6c44-132">Request</span></span>
<span data-ttu-id="a6c44-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6c44-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="a6c44-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6c44-134">Response</span></span>
<span data-ttu-id="a6c44-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6c44-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```




