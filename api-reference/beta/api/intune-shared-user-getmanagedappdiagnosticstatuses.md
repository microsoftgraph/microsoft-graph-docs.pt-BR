---
title: função getManagedAppDiagnosticStatuses
description: Obtém diagnóstico do status de validação para um determinado usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4b24f6d647612dfe142cd6fad3709c8b2186c3b4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698033"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="cdc95-103">função getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="cdc95-103">getManagedAppDiagnosticStatuses function</span></span>

<span data-ttu-id="cdc95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdc95-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cdc95-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cdc95-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cdc95-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cdc95-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cdc95-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdc95-108">Obtém diagnóstico do status de validação para um determinado usuário.</span><span class="sxs-lookup"><span data-stu-id="cdc95-108">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cdc95-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cdc95-109">Prerequisites</span></span>
<span data-ttu-id="cdc95-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdc95-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc95-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cdc95-112">Permission type</span></span>|<span data-ttu-id="cdc95-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cdc95-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cdc95-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cdc95-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="cdc95-115">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="cdc95-115">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="cdc95-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdc95-116">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cdc95-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cdc95-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cdc95-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cdc95-118">Not supported.</span></span>|
|<span data-ttu-id="cdc95-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cdc95-119">Application</span></span>||
| <span data-ttu-id="cdc95-120">&nbsp;&nbsp; **Mam**</span><span class="sxs-lookup"><span data-stu-id="cdc95-120">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="cdc95-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cdc95-121">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cdc95-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc95-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="cdc95-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc95-123">Request headers</span></span>
|<span data-ttu-id="cdc95-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cdc95-124">Header</span></span>|<span data-ttu-id="cdc95-125">Valor</span><span class="sxs-lookup"><span data-stu-id="cdc95-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cdc95-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="cdc95-126">Authorization</span></span>|<span data-ttu-id="cdc95-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cdc95-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cdc95-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cdc95-128">Accept</span></span>|<span data-ttu-id="cdc95-129">application/json</span><span class="sxs-lookup"><span data-stu-id="cdc95-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cdc95-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc95-130">Request body</span></span>
<span data-ttu-id="cdc95-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cdc95-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdc95-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc95-132">Response</span></span>
<span data-ttu-id="cdc95-133">Se tiver êxito, essa função retornará um código de resposta `200 OK` e uma coleção [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cdc95-133">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdc95-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cdc95-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="cdc95-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cdc95-135">Request</span></span>
<span data-ttu-id="cdc95-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cdc95-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="cdc95-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="cdc95-137">Response</span></span>
<span data-ttu-id="cdc95-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cdc95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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














