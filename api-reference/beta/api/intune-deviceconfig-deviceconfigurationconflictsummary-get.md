---
title: Obter deviceConfigurationConflictSummary
description: Leia as propriedades e os relacionamentos do objeto deviceConfigurationConflictSummary.
author: tfitzmac
ms.openlocfilehash: b5f38a613d10ebfd610bc8bf71bfaa30243d0d5b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333968"
---
# <a name="get-deviceconfigurationconflictsummary"></a><span data-ttu-id="ab516-103">Obter deviceConfigurationConflictSummary</span><span class="sxs-lookup"><span data-stu-id="ab516-103">Get deviceConfigurationConflictSummary</span></span>

> <span data-ttu-id="ab516-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab516-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab516-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab516-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab516-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ab516-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab516-107">Leia as propriedades e os relacionamentos do objeto [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .</span><span class="sxs-lookup"><span data-stu-id="ab516-107">Read properties and relationships of the [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab516-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab516-108">Prerequisites</span></span>
<span data-ttu-id="ab516-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab516-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab516-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab516-111">Permission type</span></span>|<span data-ttu-id="ab516-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab516-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab516-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab516-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab516-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ab516-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ab516-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab516-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab516-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab516-116">Not supported.</span></span>|
|<span data-ttu-id="ab516-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab516-117">Application</span></span>|<span data-ttu-id="ab516-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab516-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab516-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab516-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab516-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab516-120">Optional query parameters</span></span>
<span data-ttu-id="ab516-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab516-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ab516-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab516-122">Request headers</span></span>
|<span data-ttu-id="ab516-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab516-123">Header</span></span>|<span data-ttu-id="ab516-124">Valor</span><span class="sxs-lookup"><span data-stu-id="ab516-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab516-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab516-125">Authorization</span></span>|<span data-ttu-id="ab516-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab516-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab516-127">Accept</span><span class="sxs-lookup"><span data-stu-id="ab516-127">Accept</span></span>|<span data-ttu-id="ab516-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ab516-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab516-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab516-129">Request body</span></span>
<span data-ttu-id="ab516-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab516-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab516-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab516-131">Response</span></span>
<span data-ttu-id="ab516-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab516-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab516-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab516-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab516-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab516-134">Request</span></span>
<span data-ttu-id="ab516-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab516-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

### <a name="response"></a><span data-ttu-id="ab516-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab516-136">Response</span></span>
<span data-ttu-id="ab516-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab516-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 455

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
    "conflictingDeviceConfigurations": [
      {
        "@odata.type": "microsoft.graph.settingSource",
        "id": "Id value",
        "displayName": "Display Name value"
      }
    ],
    "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
    "contributingSettings": [
      "Contributing Settings value"
    ],
    "deviceCheckinsImpacted": 6
  }
}
```





