---
title: função getManagedAppDiagnosticStatuses
description: Obtém diagnóstico do status de validação para um determinado usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b9d02243cad091753083cf2019fca501229e7d24
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732276"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="839be-103">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="839be-103">getManagedAppDiagnosticStatuses function</span></span>

<span data-ttu-id="839be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="839be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="839be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="839be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="839be-106">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="839be-106">Gets diagnostics validation status for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="839be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="839be-107">Prerequisites</span></span>
<span data-ttu-id="839be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="839be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="839be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="839be-110">Permission type</span></span>|<span data-ttu-id="839be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="839be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="839be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="839be-112">Delegated (work or school account)</span></span>| <span data-ttu-id="839be-113">_varia de acordo com o contexto_</span><span class="sxs-lookup"><span data-stu-id="839be-113">_varies by context_</span></span>|
| <span data-ttu-id="839be-114">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="839be-114">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="839be-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="839be-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="839be-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="839be-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="839be-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="839be-117">Not supported.</span></span>|
|<span data-ttu-id="839be-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="839be-118">Application</span></span>|<span data-ttu-id="839be-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="839be-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="839be-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="839be-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="839be-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="839be-121">Request headers</span></span>
|<span data-ttu-id="839be-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="839be-122">Header</span></span>|<span data-ttu-id="839be-123">Valor</span><span class="sxs-lookup"><span data-stu-id="839be-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="839be-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="839be-124">Authorization</span></span>|<span data-ttu-id="839be-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="839be-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="839be-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="839be-126">Accept</span></span>|<span data-ttu-id="839be-127">application/json</span><span class="sxs-lookup"><span data-stu-id="839be-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="839be-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="839be-128">Request body</span></span>
<span data-ttu-id="839be-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="839be-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="839be-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="839be-130">Response</span></span>
<span data-ttu-id="839be-131">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="839be-131">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="839be-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="839be-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="839be-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="839be-133">Request</span></span>
<span data-ttu-id="839be-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="839be-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="839be-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="839be-135">Response</span></span>
<span data-ttu-id="839be-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="839be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









