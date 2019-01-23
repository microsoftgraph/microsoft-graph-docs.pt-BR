---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3127ca7804883c5e29fe91cf5e21bb15240a1314
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422485"
---
# <a name="update-reportroot"></a><span data-ttu-id="03b13-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="03b13-103">Update reportRoot</span></span>

> <span data-ttu-id="03b13-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="03b13-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="03b13-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="03b13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="03b13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="03b13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03b13-107">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="03b13-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="03b13-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03b13-108">Prerequisites</span></span>
<span data-ttu-id="03b13-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03b13-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03b13-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03b13-111">Permission type</span></span>|<span data-ttu-id="03b13-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03b13-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03b13-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03b13-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="03b13-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="03b13-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="03b13-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b13-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="03b13-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="03b13-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="03b13-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b13-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="03b13-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03b13-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03b13-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03b13-119">Not supported.</span></span>|
|<span data-ttu-id="03b13-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03b13-120">Application</span></span>|<span data-ttu-id="03b13-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03b13-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03b13-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03b13-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="03b13-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03b13-123">Request headers</span></span>
|<span data-ttu-id="03b13-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03b13-124">Header</span></span>|<span data-ttu-id="03b13-125">Valor</span><span class="sxs-lookup"><span data-stu-id="03b13-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03b13-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="03b13-126">Authorization</span></span>|<span data-ttu-id="03b13-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03b13-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03b13-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03b13-128">Accept</span></span>|<span data-ttu-id="03b13-129">application/json</span><span class="sxs-lookup"><span data-stu-id="03b13-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03b13-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03b13-130">Request body</span></span>
<span data-ttu-id="03b13-131">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="03b13-131">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="03b13-132">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="03b13-132">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="03b13-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03b13-133">Property</span></span>|<span data-ttu-id="03b13-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="03b13-134">Type</span></span>|<span data-ttu-id="03b13-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b13-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03b13-136">id</span><span class="sxs-lookup"><span data-stu-id="03b13-136">id</span></span>|<span data-ttu-id="03b13-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="03b13-137">String</span></span>|<span data-ttu-id="03b13-138">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="03b13-138">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="03b13-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="03b13-139">Response</span></span>
<span data-ttu-id="03b13-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03b13-140">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03b13-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03b13-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="03b13-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03b13-142">Request</span></span>
<span data-ttu-id="03b13-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03b13-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="03b13-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="03b13-144">Response</span></span>
<span data-ttu-id="03b13-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03b13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```



