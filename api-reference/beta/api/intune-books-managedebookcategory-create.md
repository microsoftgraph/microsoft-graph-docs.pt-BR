---
title: Criar managedEBookCategory
description: Crie um novo objeto de managedEBookCategory.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f86f3570f63a6aa3982e9cb2ffbf659d1a9a752c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990247"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="df3db-103">Criar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="df3db-103">Create managedEBookCategory</span></span>

> <span data-ttu-id="df3db-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="df3db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df3db-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df3db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df3db-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="df3db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df3db-107">Crie um novo objeto de [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="df3db-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df3db-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="df3db-108">Prerequisites</span></span>
<span data-ttu-id="df3db-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df3db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df3db-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="df3db-111">Permission type</span></span>|<span data-ttu-id="df3db-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="df3db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df3db-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="df3db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df3db-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df3db-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="df3db-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="df3db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df3db-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df3db-116">Not supported.</span></span>|
|<span data-ttu-id="df3db-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="df3db-117">Application</span></span>|<span data-ttu-id="df3db-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="df3db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df3db-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="df3db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="df3db-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="df3db-120">Request headers</span></span>
|<span data-ttu-id="df3db-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="df3db-121">Header</span></span>|<span data-ttu-id="df3db-122">Valor</span><span class="sxs-lookup"><span data-stu-id="df3db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df3db-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="df3db-123">Authorization</span></span>|<span data-ttu-id="df3db-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="df3db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df3db-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="df3db-125">Accept</span></span>|<span data-ttu-id="df3db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df3db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df3db-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="df3db-127">Request body</span></span>
<span data-ttu-id="df3db-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="df3db-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="df3db-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="df3db-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="df3db-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df3db-130">Property</span></span>|<span data-ttu-id="df3db-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="df3db-131">Type</span></span>|<span data-ttu-id="df3db-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="df3db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df3db-133">id</span><span class="sxs-lookup"><span data-stu-id="df3db-133">id</span></span>|<span data-ttu-id="df3db-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df3db-134">String</span></span>|<span data-ttu-id="df3db-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="df3db-135">The key of the entity.</span></span>|
|<span data-ttu-id="df3db-136">displayName</span><span class="sxs-lookup"><span data-stu-id="df3db-136">displayName</span></span>|<span data-ttu-id="df3db-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="df3db-137">String</span></span>|<span data-ttu-id="df3db-138">O nome da categoria eBook.</span><span class="sxs-lookup"><span data-stu-id="df3db-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="df3db-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df3db-139">lastModifiedDateTime</span></span>|<span data-ttu-id="df3db-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df3db-140">DateTimeOffset</span></span>|<span data-ttu-id="df3db-141">A data e a hora que da última modificação do ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="df3db-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="df3db-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="df3db-142">Response</span></span>
<span data-ttu-id="df3db-143">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="df3db-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df3db-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="df3db-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="df3db-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="df3db-145">Request</span></span>
<span data-ttu-id="df3db-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="df3db-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="df3db-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="df3db-147">Response</span></span>
<span data-ttu-id="df3db-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="df3db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





