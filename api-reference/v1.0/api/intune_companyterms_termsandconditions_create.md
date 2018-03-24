# <a name="create-termsandconditions"></a><span data-ttu-id="26b13-101">Criar termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="26b13-101">Create termsAndConditions</span></span>

> <span data-ttu-id="26b13-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="26b13-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="26b13-103">Criar um novo objeto [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).</span><span class="sxs-lookup"><span data-stu-id="26b13-103">Create a new [plannerBucket](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="26b13-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26b13-104">Prerequisites</span></span>
<span data-ttu-id="26b13-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="26b13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="26b13-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26b13-107">Permission type</span></span>|<span data-ttu-id="26b13-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26b13-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26b13-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26b13-109">Delegated (work or school account)</span></span>|<span data-ttu-id="26b13-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26b13-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26b13-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26b13-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26b13-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26b13-112">Not supported.</span></span>|
|<span data-ttu-id="26b13-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26b13-113">Application</span></span>|<span data-ttu-id="26b13-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26b13-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26b13-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26b13-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="26b13-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26b13-116">Request headers</span></span>
|<span data-ttu-id="26b13-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26b13-117">Header</span></span>|<span data-ttu-id="26b13-118">Valor</span><span class="sxs-lookup"><span data-stu-id="26b13-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26b13-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="26b13-119">Authorization</span></span>|<span data-ttu-id="26b13-120">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26b13-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="26b13-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26b13-121">Accept</span></span>|<span data-ttu-id="26b13-122">application/json</span><span class="sxs-lookup"><span data-stu-id="26b13-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26b13-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26b13-123">Request body</span></span>
<span data-ttu-id="26b13-124">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="26b13-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="26b13-125">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditions.</span><span class="sxs-lookup"><span data-stu-id="26b13-125">The following table shows the properties that are required when you create a invitation.</span></span>

|<span data-ttu-id="26b13-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26b13-126">Property</span></span>|<span data-ttu-id="26b13-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="26b13-127">Type</span></span>|<span data-ttu-id="26b13-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="26b13-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26b13-129">id</span><span class="sxs-lookup"><span data-stu-id="26b13-129">id</span></span>|<span data-ttu-id="26b13-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26b13-130">String</span></span>|<span data-ttu-id="26b13-131">Identificador exclusivo da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="26b13-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="26b13-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26b13-132">createdDateTime</span></span>|<span data-ttu-id="26b13-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26b13-133">DateTimeOffset</span></span>|<span data-ttu-id="26b13-134">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="26b13-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="26b13-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26b13-135">lastModifiedDateTime</span></span>|<span data-ttu-id="26b13-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26b13-136">DateTimeOffset</span></span>|<span data-ttu-id="26b13-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="26b13-137">Indicates the date the object was last modified.</span></span>|
|<span data-ttu-id="26b13-138">displayName</span><span class="sxs-lookup"><span data-stu-id="26b13-138">displayName</span></span>|<span data-ttu-id="26b13-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26b13-139">String</span></span>|<span data-ttu-id="26b13-140">Nome fornecido pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="26b13-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="26b13-141">descrição</span><span class="sxs-lookup"><span data-stu-id="26b13-141">description</span></span>|<span data-ttu-id="26b13-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26b13-142">String</span></span>|<span data-ttu-id="26b13-143">Descrição fornecida pelo administrador para a política de T&C.</span><span class="sxs-lookup"><span data-stu-id="26b13-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="26b13-144">title</span><span class="sxs-lookup"><span data-stu-id="26b13-144">title</span></span>|<span data-ttu-id="26b13-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26b13-145">String</span></span>|<span data-ttu-id="26b13-146">Título dos termos e condições fornecido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="26b13-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="26b13-147">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="26b13-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="26b13-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="26b13-148">bodyText</span></span>|<span data-ttu-id="26b13-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26b13-149">String</span></span>|<span data-ttu-id="26b13-150">Corpo de texto de termos e condições fornecido pelo administrador, normalmente os termos em si.</span><span class="sxs-lookup"><span data-stu-id="26b13-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="26b13-151">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="26b13-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="26b13-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="26b13-152">acceptanceStatement</span></span>|<span data-ttu-id="26b13-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26b13-153">String</span></span>|<span data-ttu-id="26b13-154">Explicação dos termos e condições fornecida pelo administrador, normalmente para descrever o que significa aceitar os termos e condições definidos na política de T&C.</span><span class="sxs-lookup"><span data-stu-id="26b13-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="26b13-155">Isso é exibido ao usuário nos prompts de aceitação da política de T&C.</span><span class="sxs-lookup"><span data-stu-id="26b13-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="26b13-156">version</span><span class="sxs-lookup"><span data-stu-id="26b13-156">version</span></span>|<span data-ttu-id="26b13-157">Int32</span><span class="sxs-lookup"><span data-stu-id="26b13-157">Int32</span></span>|<span data-ttu-id="26b13-158">Inteiro que indica a versão atual dos termos.</span><span class="sxs-lookup"><span data-stu-id="26b13-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="26b13-159">Incrementado quando um administrador faz uma alteração nos termos e deseja solicitar que os usuários aceitem novamente a política de T&C modificada.</span><span class="sxs-lookup"><span data-stu-id="26b13-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="26b13-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="26b13-160">Response</span></span>
<span data-ttu-id="26b13-161">Se tiver êxito, este método retornará o código de resposta `201 Created` e um objeto [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26b13-161">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26b13-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26b13-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="26b13-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26b13-163">Request</span></span>
<span data-ttu-id="26b13-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26b13-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 337

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="26b13-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="26b13-165">Response</span></span>
<span data-ttu-id="26b13-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26b13-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



