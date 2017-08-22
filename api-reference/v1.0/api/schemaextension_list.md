# <a name="list-schemaextensions"></a><span data-ttu-id="38194-101">Listar schemaExtensions</span><span class="sxs-lookup"><span data-stu-id="38194-101">List schemaExtensions</span></span>

<span data-ttu-id="38194-102">Obtenha uma lista de objetos [schemaExtension](../resources/schemaextension.md) criados por aplicativos que você possui no locatário atual (que pode ser **InDevelopment**, **Available** ou **Deprecated**) e todas as outras extensões de esquema pertencentes a outros aplicativos que estão marcadas como **Available**.</span><span class="sxs-lookup"><span data-stu-id="38194-102">Get a list of [schemaExtension](../resources/schemaextension.md) objects created by any apps you own in the current tenant (that can be **InDevelopment**, **Available**, or **Deprecated**), and all other schema extensions owned by other apps that are marked as **Available**.</span></span> 

## <a name="prerequisites"></a><span data-ttu-id="38194-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38194-103">Prerequisites</span></span>
<span data-ttu-id="38194-104">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="38194-104">One of the following **scopes** is required to execute this API: *Directory.Read.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="38194-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38194-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="38194-106">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="38194-106">Optional query parameters</span></span>
<span data-ttu-id="38194-107">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="38194-107">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="38194-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38194-108">Request headers</span></span>
| <span data-ttu-id="38194-109">Nome</span><span class="sxs-lookup"><span data-stu-id="38194-109">Name</span></span>      |<span data-ttu-id="38194-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="38194-110">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38194-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="38194-111">Authorization</span></span>  | <span data-ttu-id="38194-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38194-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="38194-114">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38194-114">Content-Type</span></span>   | <span data-ttu-id="38194-115">application/json</span><span class="sxs-lookup"><span data-stu-id="38194-115">application/json</span></span> | 

## <a name="request-body"></a><span data-ttu-id="38194-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38194-116">Request body</span></span>
<span data-ttu-id="38194-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="38194-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38194-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="38194-118">Response</span></span>

<span data-ttu-id="38194-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [schemaExtension](../resources/schemaextension.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38194-119">If successful, this method returns a `200 OK` response code and collection of [schemaExtension](../resources/schemaextension.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38194-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38194-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38194-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38194-121">Request</span></span>
<span data-ttu-id="38194-122">O exemplo a seguir mostra como procurar entre todas as extensões acessíveis uma que seja específica ao filtrar sua **id** exclusiva.</span><span class="sxs-lookup"><span data-stu-id="38194-122">The following example shows how to look among all the accessible extensions for a specific one by filtering on its unique **id**.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="38194-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="38194-123">Response</span></span>
<span data-ttu-id="38194-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38194-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
    {
      "id":"graphlearn_test",
      "description": "Yet another test schema",
      "targetTypes": [
          "User", "Group"
      ],
      "status": "InDevelopment",
      "owner": "24d3b144-21ae-4080-943f-7067b395b913",
      "properties": [
          {
              "name": "testName",
              "type": "String"
          }
      ]
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="38194-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="38194-127">See also</span></span>

- [<span data-ttu-id="38194-128">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="38194-128">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="38194-129">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="38194-129">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->