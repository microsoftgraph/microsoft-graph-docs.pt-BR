# <a name="security-resource-type"></a>tipo de recurso Security

O recurso Security é o ponto de entrada para o modelo de objeto de segurança. Ele retorna um recurso security singleton. Não contém nenhuma propriedade utilizável.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [List alertas](../api/alert_list.md) | coleção [alert](alert.md) | Obtém uma coleção de objetos alert. |
| [get alerts](../api/alert_get.md) | coleção [alert](alert.md) | Obtém um objeto alert. |
| [Update alerts](../api/alert_update.md) | coleção [alert](alert.md) | Obtém um objeto alert. |

## <a name="properties"></a>Propriedades
Nenhum

## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|alerts|coleção [alert](alert.md)| Somente leitura. Anulável.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a>Exemplo

O recurso **security** está disponível na raiz do gráfico.

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->