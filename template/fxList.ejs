import React, { useEffect, useState } from 'react'
import MainLayout from '@/layout/mainLayout'
import { Form, Input, Button, Select, DatePicker, Space, Menu, Tooltip } from 'antd'
import './index.less'
import { deal_status } from '@/config/maps/maps'
import { Link } from 'react-router-dom'
import { formatDate, formatNumber, formatStateToForm } from '@/utils/utils'
import MyTable from '@/components/my-table'
import { ExportOutlined } from '@ant-design/icons'

const { RangePicker } = DatePicker
const { Option } = Select

const initialValues = {}

const sortMap = {}

export default function <%= data.name %>() {
  const [form] = Form.useForm()
  const [searchParams, setSearchParams] = useState(getSearchParamsInitialValues)
  const [sortParams, setSortParams] = useState({})
  const fixedParams = {}
  function formatBody(values) {
    const body = { ...values }

    // body.amountFrom = body.amount?.start;
    // body.amountTo = body?.amount?.end;
    // delete body.amount;

    // if (body.dates?.length > 0) {
    //   body.queryDateFrom = body?.dates?.[0].startOf('day').format('YYYY-MM-DD HH:mm:ss');
    //   body.queryDateTo = body?.dates?.[1].endOf('day').format('YYYY-MM-DD HH:mm:ss');
    //   delete body.dates
    // }
    return body
  }

  //获取SearchParams初始值
  function getSearchParamsInitialValues() {
    return location.state ? formatBody(formatStateToForm(location.state)) : initialValues
  }

  const onSearch = values => {
    setSearchParams(formatBody(values))
  }

  const onReset = () => {
    form.resetFields()
    setSearchParams(form.getFieldsValue())
  }

  const columns = [
    {
      title: 'Column1',
      dataIndex: 'column1',
      render(id, record) {
        return <Link to={`/xx`}>{record.code}</Link>
      },
    },
    { title: 'Column2', dataIndex: 'column2' },
    {
      title: 'Column3',
      dataIndex: 'column3',
    },
    {
      title: 'Column4',
      dataIndex: 'column4',
      ellipsis: {
        showTitle: false,
      },
    },
    { title: 'Column5', dataIndex: 'column5', sorter: true, render: text => formatDate(text) },
    {
      width: 120,
      title: 'Action',
      render: record => (
        <Space size='middle'>
          <Link to={`/deal/request-detail/${record.id}`}>Btn1</Link>
          <Link to={`/deal/request-detail/${record.id}`}>Btn2</Link>
        </Space>
      ),
    },
  ]

  return (
    <MainLayout title='FX Deals' className='deal-list'>
      <div className='my-wrap'>
        <Form
          form={form}
          labelCol={{ span: 8 }}
          wrapperCol={{ span: 16 }}
          layout='inline'
          initialValues={initialValues}
          onFinish={onSearch}
          className={'search-form'}
          colon={false}
          size={'large'}
        >
          <Form.Item label='Field1' name='field1'>
            <Select style={{ width: 120 }} placeholder='Date Style' options={[]}></Select>
          </Form.Item>
          <Form.Item label='Field2' name='field1'>
            <RangePicker style={{ width: 300 }} />
          </Form.Item>

          <Form.Item label='Field3' name='field3'>
            <Input style={{ width: 256 }} />
          </Form.Item>
          <Form.Item className={'search-form-btn'}>
            <Button type='primary' htmlType='submit'>
              Search
            </Button>
          </Form.Item>

          <Form.Item className={'search-form-btn'}>
            <Button onClick={onReset}>Reset</Button>
          </Form.Item>

          {/*<Form.Item>*/}
          {/*  <a>Export</a>*/}
          {/*</Form.Item>*/}
        </Form>
        <div className='my-divider' />
        <div className='btn-list' style={{ textAlign: 'right' }}>
          <Space>
            <Button
              type={'link'}
              size={'large'}
              icon={<ExportOutlined style={{ fontSize: 16, position: 'relative', top: '1px' }} />}
            >
              Export
            </Button>
          </Space>
        </div>
        <MyTable
          searchParams={searchParams}
          fixedParams={fixedParams}
          url='/admin/busi/v1/deal/query'
          rowKey='id'
          columns={columns}
          resDataFiled={'dealVOList'}
          sortMap={sortMap}
          onSortChange={v => setSortParams(v)}
          cacheConfig={{
            form,
          }}
        />
      </div>
    </MainLayout>
  )
}
