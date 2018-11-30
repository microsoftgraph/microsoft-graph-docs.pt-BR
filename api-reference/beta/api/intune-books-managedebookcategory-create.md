---
title: Criar managedEBookCategory
description: Crie um novo objeto de managedEBookCategory.
ms.openlocfilehash: 8750e8c520e3a48b2da93d05b9f701c7760b6a15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039519"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="27ea4-103">Criar managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="27ea4-103">Create managedEBookCategory</span></span>

> <span data-ttu-id="27ea4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="27ea4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27ea4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="27ea4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27ea4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="27ea4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27ea4-107">Crie um novo objeto de [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="27ea4-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27ea4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="27ea4-108">Prerequisites</span></span>
<span data-ttu-id="27ea4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27ea4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27ea4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="27ea4-111">Permission type</span></span>|<span data-ttu-id="27ea4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="27ea4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27ea4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="27ea4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27ea4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27ea4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27ea4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="27ea4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27ea4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27ea4-116">Not supported.</span></span>|
|<span data-ttu-id="27ea4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="27ea4-117">Application</span></span>|<span data-ttu-id="27ea4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="27ea4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27ea4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="27ea4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="27ea4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="27ea4-120">Request headers</span></span>
|<span data-ttu-id="27ea4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="27ea4-121">Header</span></span>|<span data-ttu-id="27ea4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="27ea4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27ea4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="27ea4-123">Authorization</span></span>|<span data-ttu-id="27ea4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="27ea4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27ea4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="27ea4-125">Accept</span></span>|<span data-ttu-id="27ea4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27ea4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27ea4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="27ea4-127">Request body</span></span>
<span data-ttu-id="27ea4-128">No corpo da solicitação, fornece uma representação JSON para o objeto managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="27ea4-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="27ea4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="27ea4-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="27ea4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="27ea4-130">Property</span></span>|<span data-ttu-id="27ea4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="27ea4-131">Type</span></span>|<span data-ttu-id="27ea4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="27ea4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27ea4-133">id</span><span class="sxs-lookup"><span data-stu-id="27ea4-133">id</span></span>|<span data-ttu-id="27ea4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="27ea4-134">String</span></span>|<span data-ttu-id="27ea4-135">A chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="27ea4-135">The key of the entity.</span></span>|
|<span data-ttu-id="27ea4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="27ea4-136">displayName</span></span>|<span data-ttu-id="27ea4-137">String</span><span class="sxs-lookup"><span data-stu-id="27ea4-137">String</span></span>|<span data-ttu-id="27ea4-138">O nome da categoria eBook.</span><span class="sxs-lookup"><span data-stu-id="27ea4-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="27ea4-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27ea4-139">lastModifiedDateTime</span></span>|<span data-ttu-id="27ea4-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27ea4-140">DateTimeOffset</span></span>|<span data-ttu-id="27ea4-141">A data e a hora que da última modificação do ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="27ea4-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="27ea4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="27ea4-142">Response</span></span>
<span data-ttu-id="27ea4-143">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [managedEBookCategory](../resources/intune-books-managedebookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="27ea4-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27ea4-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="27ea4-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="27ea4-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="27ea4-145">Request</span></span>
<span data-ttu-id="27ea4-146">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="27ea4-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27ea4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="27ea4-147">Response</span></span>
<span data-ttu-id="27ea4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="27ea4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





