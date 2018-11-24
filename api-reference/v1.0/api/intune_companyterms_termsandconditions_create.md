# <a name="create-termsandconditions"></a><span data-ttu-id="3fd27-101">Criar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="3fd27-101">Create termsAndConditions</span></span>

> <span data-ttu-id="3fd27-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3fd27-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fd27-103">Criar um novo objeto [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="3fd27-103">Create a new [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3fd27-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3fd27-104">Prerequisites</span></span>
<span data-ttu-id="3fd27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="3fd27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3fd27-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fd27-107">Permission type</span></span>|<span data-ttu-id="3fd27-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3fd27-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fd27-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fd27-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3fd27-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fd27-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3fd27-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fd27-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fd27-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fd27-112">Not supported.</span></span>|
|<span data-ttu-id="3fd27-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fd27-113">Application</span></span>|<span data-ttu-id="3fd27-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fd27-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fd27-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fd27-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="3fd27-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fd27-116">Request headers</span></span>
|<span data-ttu-id="3fd27-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fd27-117">Header</span></span>|<span data-ttu-id="3fd27-118">Valor</span><span class="sxs-lookup"><span data-stu-id="3fd27-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fd27-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fd27-119">Authorization</span></span>|<span data-ttu-id="3fd27-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fd27-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fd27-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3fd27-121">Accept</span></span>|<span data-ttu-id="3fd27-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3fd27-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fd27-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fd27-123">Request body</span></span>
<span data-ttu-id="3fd27-124">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="3fd27-124">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="3fd27-125">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="3fd27-125">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="3fd27-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fd27-126">Property</span></span>|<span data-ttu-id="3fd27-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fd27-127">Type</span></span>|<span data-ttu-id="3fd27-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fd27-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fd27-129">id</span><span class="sxs-lookup"><span data-stu-id="3fd27-129">id</span></span>|<span data-ttu-id="3fd27-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fd27-130">String</span></span>|<span data-ttu-id="3fd27-131">Identificador exclusivo da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="3fd27-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="3fd27-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3fd27-132">createdDateTime</span></span>|<span data-ttu-id="3fd27-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fd27-133">DateTimeOffset</span></span>|<span data-ttu-id="3fd27-134">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3fd27-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="3fd27-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fd27-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3fd27-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fd27-136">DateTimeOffset</span></span>|<span data-ttu-id="3fd27-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3fd27-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3fd27-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3fd27-138">displayName</span></span>|<span data-ttu-id="3fd27-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fd27-139">String</span></span>|<span data-ttu-id="3fd27-140">Nome fornecido pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="3fd27-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="3fd27-141">descrição</span><span class="sxs-lookup"><span data-stu-id="3fd27-141">description</span></span>|<span data-ttu-id="3fd27-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fd27-142">String</span></span>|<span data-ttu-id="3fd27-143">Descrição fornecida pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="3fd27-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="3fd27-144">title</span><span class="sxs-lookup"><span data-stu-id="3fd27-144">title</span></span>|<span data-ttu-id="3fd27-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fd27-145">String</span></span>|<span data-ttu-id="3fd27-146">Título dos termos e condições fornecido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3fd27-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="3fd27-147">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="3fd27-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3fd27-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="3fd27-148">bodyText</span></span>|<span data-ttu-id="3fd27-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fd27-149">String</span></span>|<span data-ttu-id="3fd27-150">Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si.</span><span class="sxs-lookup"><span data-stu-id="3fd27-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="3fd27-151">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="3fd27-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3fd27-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="3fd27-152">acceptanceStatement</span></span>|<span data-ttu-id="3fd27-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fd27-153">String</span></span>|<span data-ttu-id="3fd27-154">Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C.</span><span class="sxs-lookup"><span data-stu-id="3fd27-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="3fd27-155">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="3fd27-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="3fd27-156">version</span><span class="sxs-lookup"><span data-stu-id="3fd27-156">version</span></span>|<span data-ttu-id="3fd27-157">Int32</span><span class="sxs-lookup"><span data-stu-id="3fd27-157">Int32</span></span>|<span data-ttu-id="3fd27-158">Inteiro que indica a versão atual dos termos.</span><span class="sxs-lookup"><span data-stu-id="3fd27-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="3fd27-159">Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.</span><span class="sxs-lookup"><span data-stu-id="3fd27-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="3fd27-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fd27-160">Response</span></span>
<span data-ttu-id="3fd27-161">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fd27-161">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fd27-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fd27-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="3fd27-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fd27-163">Request</span></span>
<span data-ttu-id="3fd27-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fd27-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="3fd27-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fd27-165">Response</span></span>
<span data-ttu-id="3fd27-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3fd27-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



