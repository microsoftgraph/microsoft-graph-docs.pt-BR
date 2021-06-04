---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d67e334b0f9ff3329bfa3bdfbd5436527461d9f
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732294"
---
# <a name="update-reportroot"></a><span data-ttu-id="b6969-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="b6969-103">Update reportRoot</span></span>

<span data-ttu-id="b6969-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6969-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6969-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6969-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6969-106">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b6969-106">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6969-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6969-107">Prerequisites</span></span>
<span data-ttu-id="b6969-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6969-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6969-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6969-110">Permission type</span></span>|<span data-ttu-id="b6969-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6969-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6969-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6969-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b6969-113">&nbsp;&nbsp;Configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b6969-113">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="b6969-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6969-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b6969-115">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="b6969-115">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="b6969-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6969-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b6969-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6969-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6969-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6969-118">Not supported.</span></span>|
|<span data-ttu-id="b6969-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6969-119">Application</span></span>|<span data-ttu-id="b6969-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6969-120">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6969-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6969-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="b6969-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6969-122">Request headers</span></span>
|<span data-ttu-id="b6969-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6969-123">Header</span></span>|<span data-ttu-id="b6969-124">Valor</span><span class="sxs-lookup"><span data-stu-id="b6969-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6969-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6969-125">Authorization</span></span>|<span data-ttu-id="b6969-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6969-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6969-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6969-127">Accept</span></span>|<span data-ttu-id="b6969-128">application/json</span><span class="sxs-lookup"><span data-stu-id="b6969-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6969-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6969-129">Request body</span></span>
<span data-ttu-id="b6969-130">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b6969-130">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="b6969-131">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b6969-131">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="b6969-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6969-132">Property</span></span>|<span data-ttu-id="b6969-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6969-133">Type</span></span>|<span data-ttu-id="b6969-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6969-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6969-135">id</span><span class="sxs-lookup"><span data-stu-id="b6969-135">id</span></span>|<span data-ttu-id="b6969-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6969-136">String</span></span>|<span data-ttu-id="b6969-137">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="b6969-137">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b6969-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6969-138">Response</span></span>
<span data-ttu-id="b6969-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6969-139">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6969-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6969-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6969-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6969-141">Request</span></span>
<span data-ttu-id="b6969-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6969-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="b6969-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6969-143">Response</span></span>
<span data-ttu-id="b6969-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6969-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```














